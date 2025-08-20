# Copilot custom chat modes

Custom [Copilot chatmodes](https://code.visualstudio.com/docs/copilot/chat/chat-modes) for structured workflows. Largely based on agents and templates from [claude-code-spec-workflow](https://github.com/Pimzino/claude-code-spec-workflow) and adapted for Copilot chatmodes.

Feature implementation: **Requirements → Design → Tasks → Implementation -> Review -> Fixes**

Bug fixing: **Analysis → Fixing**

## Feature implementation

### All-in-one spec creation

Use `Spec-creator` to create all three documents (requirements, design, and tasks) using single chatmode. More streamlined, but will use more context. Good for smaller features/codebases.

Prompt example: "Create spec documents for X feature"

### 3-step spec creation

Use `Spec(1)-requirements`, `Spec(2)-design`, and `Spec(3)-tasks` in this order, as each step builds on the previous one to create requirements, design, and tasks documents in separate chats. Good for larger features/codebases.

Requirements prompt example: "Create requirements for X feature"  
Design prompt example: "Create design for {feature-name}"  
Tasks prompt example: "Create tasks for {feature-name}"

### Task execution

Use `Spec-task-executor` to execute tasks created in the previous step.

Example prompt: "Execute task X for {feature-name}"

### Implementation review (optional)

Use `Implementation-reviewer` to review the implementation of the feature. This will create a report document where you can provide additional feedback.

Example prompt: "Review implementation for {feature-name}"

### Implementation fixes and changes (optional)

Use `Implementation-fixer` to make changes to the implementation based on the review feedback document.

Example prompt: "Address issues identified in {feature-name} implementation review"

## Bug fixing

### Bug analysis

Use `Bug-analyzer` to analyze the bug and gather relevant information. It will create a bug analysis document for `Bug-fixer` to use.

### Fixing

Use `Bug-fixer` to fix the bug based on the analysis document.
