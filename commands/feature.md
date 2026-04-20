---
description: Design and implement a new feature
argument-hint: [feature-description]
---

# /ai-msdt:feature

## Goal
Design and implement a new feature from specification to working code.

## Instructions

### 1. Requirements analysis
- Understand the feature's goal and business value
- Identify users and use cases
- Determine dependencies on existing code

### 2. Design
- Propose a solution architecture (components, interfaces, data flow)
- List files to modify and new files to create
- Describe the public API contract

### 3. Implementation
- Write code consistent with project conventions
- Apply design patterns appropriate to the problem
- Handle errors and validate inputs at system boundaries

### 4. Tests
- Write unit tests for critical logic
- Cover happy path, edge cases, and error handling
- Use the AAA pattern (Arrange-Act-Assert)

## Rules
- Do not add code outside the task scope
- Code must be secure (no SQL injection, XSS, command injection)
- Minimal complexity — three similar lines beat a premature abstraction
- No feature flags or backwards-compatibility shims unless explicitly required

## Output format
1. **Summary** — what will be built and why
2. **Change plan** — list of files with a short description of each change
3. **Code** — implementation with line numbers
4. **Tests** — tests for the new functionality
