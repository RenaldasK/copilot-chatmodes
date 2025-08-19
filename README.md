# Copilot custom chat modes

Custom [Copilot chatmodes](https://code.visualstudio.com/docs/copilot/chat/chat-modes) for structured workflows. Largely based on agents and templates from [claude-code-spec-workflow](https://github.com/Pimzino/claude-code-spec-workflow) and adapted for Copilot chatmodes.

Feature implementation: **Requirements → Design → Tasks → Implementation -> Review -> Fixes**

Bug fixing: **Analysis → Fixing**

## Feature implementation

### All-in-one spec creation

Use `Spec-creator` to create all three documents (spec, design, and tasks) using single chatmode. More streamlined, but will use more context. Good for smaller features/codebases.

### 3-step spec creation

Use `Spec(1)-requirements`, `Spec(2)-design`, and `Spec(3)-tasks` in this order, as each step builds on the previous one to create spec, design, and tasks documents in separate chats. Good for larger features/codebases.

### Task execution

Use `Spec-task-executor` to execute tasks created in the previous step.

### Implementation review (optional)

Use `Implementation-reviewer` to review the implementation of the feature. This will create a report document where you can provide additional feedback.

### Implementation fixes and changes (optional)

Use `Implementation-fixer` to make changes to the implementation based on the review feedback document.

## Bug fixing

### Bug analysis

Use `Bug-analyzer` to analyze the bug and gather relevant information.

### Fixing

Use `Bug-fixer` to fix the bug based on the analysis document.
