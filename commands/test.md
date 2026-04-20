---
description: Write tests for the specified code
argument-hint: [file-path]
---

# /ai-msdt:test

## Goal
Write unit tests for the specified code.

## Instructions
1. Identify the public API to test
2. Determine edge cases and boundary conditions
3. Write tests using the appropriate framework for the stack
4. Follow the AAA pattern (Arrange-Act-Assert)

## Rules
- Test names describe behaviour: `Should_DoSomething_When_Condition`
- One reason to fail per test
- Cover: happy path, edge cases, error handling
