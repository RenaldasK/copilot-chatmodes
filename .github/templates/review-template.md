# Code Review Report

## Review Summary

**Feature**: [Feature name and brief description]
**Review Date**: [Date]
**Overall Status**: [APPROVED | NEEDS_FIXES | MAJOR_ISSUES]

[Provide a high-level summary of the review findings and recommendation]

## Requirements Validation

### Complete Satisfaction Check

- [ ] All user stories from requirements.md are fully implemented
- [ ] All acceptance criteria have been met
- [ ] Feature delivers intended business value

**Issues Found**:
[List any requirements not met or partially implemented]

### Edge Case Coverage

- [ ] Error scenarios are properly handled
- [ ] Boundary conditions are tested
- [ ] Invalid input handling is implemented

**Missing Edge Cases**:
[List any edge cases that need attention]

## Design Implementation Verification

### Architecture Compliance

- [ ] Implementation follows specified architecture from design.md
- [ ] Component interactions match design specifications
- [ ] Data flow aligns with architectural decisions

**Architecture Deviations**:
[List any deviations from the specified architecture]

### API Contract Adherence

- [ ] API endpoints match design specifications
- [ ] Request/response formats are correct
- [ ] Error responses follow specified patterns

### Data Model Consistency

- [ ] Database schema matches design specifications
- [ ] Data relationships are properly implemented

## Task Completion Audit

### Implementation Completeness

- [ ] All tasks from tasks.md are fully implemented
- [ ] Task interdependencies are properly handled
- [ ] Success criteria for each task are met

**Incomplete Tasks**:
[List any tasks that are missing or partially implemented]

### Integration Verification

- [ ] Task outputs integrate properly with each other
- [ ] No missing connections between task implementations
- [ ] End-to-end workflow functions correctly

## Code Quality Assessment

### Overall Quality Score

**Rating**: [1-5, where 5 is excellent]
**Justification**: [Brief explanation of the rating]

### Quality Issues Found

#### Critical Issues

[List any issues that must be fixed before merge]

#### Major Issues

[List any issues that should be fixed before merge]

#### Minor Issues

[List any issues that can be addressed in follow-up work]

### Consistency Analysis

- [ ] Coding patterns are consistent across the implementation
- [ ] Naming conventions are followed
- [ ] Code structure follows established patterns

### Error Handling Review

- [ ] Comprehensive error handling is implemented
- [ ] Error messages are user-friendly and informative
- [ ] Graceful degradation is implemented where appropriate

### Security Assessment

- [ ] Input validation is properly implemented
- [ ] Authentication/authorization checks are in place
- [ ] Security best practices are followed
- [ ] No sensitive data is exposed

**Security Concerns**:

[List any security issues found]

## Code Duplication Analysis

### Duplication Detection Results

#### Exact Duplicates Found

[List any identical code blocks with locations]

- **Location 1**: `file1.ext:lines X-Y`
- **Location 2**: `file2.ext:lines A-B`
- **Duplication Type**: [Exact/Similar/Functional]

#### Similar Patterns Identified

[List structurally similar code sections]

#### Semantic Duplicates

[List code that performs the same function differently]

### Refactoring Recommendations

#### High Priority Refactoring

1. **Extract Method**: [Description]
   - **Files Affected**: [List files]
   - **Benefits**: [Maintenance, readability, etc.]
2. **Create Utility Functions**: [Description]
   - **Common Functionality**: [What can be shared]
   - **Suggested Location**: [Where to place utilities]

#### Medium Priority Refactoring

[List medium priority refactoring opportunities]

#### Low Priority Refactoring

[List nice-to-have refactoring opportunities]

### Duplication Impact Assessment

- **Maintenance Impact**: [How duplication affects future maintenance]
- **Bug Propagation Risk**: [Risk of bugs appearing in multiple places]
- **Technical Debt Score**: [Quantified assessment]
- **Refactoring Effort Estimate**: [Time/complexity estimate]

## Performance Analysis

### Algorithmic Complexity Assessment

#### Time Complexity Issues

[List functions with concerning time complexity]

- **Function**: `functionName()` in `file.ext`
- **Current Complexity**: O(n²)
- **Issue**: [Description of the performance problem]
- **Suggested Improvement**: [Alternative approach]
- **Expected Complexity**: O(n log n)

#### Space Complexity Issues

[List memory usage concerns]

#### Recursive Function Analysis

[Analysis of recursive functions and stack overflow risks]

### Performance Bottlenecks Identified

#### Database Performance

- [ ] N+1 query problems detected
- [ ] Missing database indexes identified
- [ ] Inefficient query patterns found

**Database Issues**:

[Include actual queries or query patterns]

#### Network Performance

- [ ] Excessive API calls identified
- [ ] Missing request batching opportunities
- [ ] Inefficient data fetching patterns

#### Memory Performance

- [ ] Potential memory leaks identified
- [ ] Inefficient data structures used
- [ ] Large object retention issues

#### CPU Performance

- [ ] Computation-heavy sections identified
- [ ] Inefficient algorithms detected
- [ ] Missing optimization opportunities

### Optimization Recommendations

#### High Impact Optimizations

1. **Optimization**: [Description]
   - **Current Performance**: [Metrics]
   - **Expected Improvement**: [Expected metrics]
   - **Implementation Effort**: [Effort estimate]
   - **Risk Level**: [Low/Medium/High]

#### Caching Opportunities

[List areas where caching would improve performance]

#### Parallel Processing Opportunities

[Identify code that could benefit from parallelization]

### Performance Testing Recommendations

#### Benchmark Suggestions

[Recommend specific performance tests]

#### Profiling Points

[Suggest where to add performance monitoring]

#### Performance Budgets

[Define acceptable performance thresholds]

## Risk Assessment

### High Risk Issues

[Issues that could cause production problems]

### Medium Risk Issues

[Issues that should be monitored]

### Low Risk Issues

[Minor issues for future consideration]

## Action Items

### Must Fix Before Merge (Critical Issues)

1. [ ] [Critical issue requiring immediate attention]
2. [ ] [Another critical issue]

### Should Fix Before Merge (Major Issues)

1. [ ] [Important issue that should be addressed]
2. [ ] [Another important issue]

### Follow-up Items (Minor Issues and Improvements)

1. [ ] [Technical debt item for future sprints]
2. [ ] [Performance optimization for later]

## Review Conclusion

### Summary

[Overall assessment of the code review]

### Recommendation

[Final recommendation: approve, request changes, etc.]

### Next Steps

[What should happen next in the review process]

---

### Review Metadata

- **Files Reviewed**: [Number]
- **Complexity Score**: [Overall complexity assessment]
