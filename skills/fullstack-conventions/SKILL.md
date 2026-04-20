---
name: fullstack-conventions
description: Conventions and patterns for fullstack projects (.NET, React, Angular, Go, TS, Python)
globs: ["**/*.cs", "**/*.ts", "**/*.tsx", "**/*.vue", "**/*.go", "**/*.py", "**/*.jsx"]
---

# Fullstack Conventions

## Project structure
- Separate layers: transport → business logic → data
- Feature-based structure for frontends
- Clean Architecture for .NET

## Naming
- **Classes/types**: PascalCase
- **Functions/methods**: camelCase (TS/Go), snake_case (Python), PascalCase (.NET)
- **Variables**: camelCase (TS/Go/.NET), snake_case (Python)
- **Constants**: SCREAMING_SNAKE_CASE
- **Component files**: PascalCase (React/Angular/Vue)

## Error handling
- Prefer Result pattern over exceptions where possible
- Log with context (correlation ID, user ID)
- Never swallow errors — propagate to the layer above

## API
- RESTful: nouns, HTTP verbs, correct status codes
- Always paginate lists
- Version via URL path

## Tests
- AAA pattern (Arrange-Act-Assert)
- Test names describe behaviour
- 70% unit / 20% integration / 10% E2E

## Git
- Conventional commits: feat/fix/refactor/docs/test/chore
- Small, atomic commits
- Branch per feature
