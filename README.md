# AI-MSDT (Multi-Stack Development Toolkit)

Claude Code CLI plugin with agents and tools for fullstack developers.

## Stack

- .NET / C#
- React / Angular / Vue
- TypeScript
- Go
- Python

## Contents

### Agents (12)

| Agent | Description |
|-------|-------------|
| `architect` | System architect |
| `api-designer` | API designer (REST/gRPC) |
| `code-reviewer` | Code reviewer |
| `refactor-advisor` | Refactoring advisor |
| `test-engineer` | Test engineer |
| `security-auditor` | Security auditor |
| `db-architect` | Database architect |
| `devops-engineer` | DevOps engineer |
| `docs-writer` | Technical writer |
| `debugger` | Debugger / diagnostician |
| `performance-tuner` | Performance specialist |
| `ux-consultant` | UX consultant |

### Commands

- `/ai-msdt:review [file]` — code review
- `/ai-msdt:explain [file]` — explain code
- `/ai-msdt:test [file]` — generate tests
- `/ai-msdt:feature [description]` — design and implement a feature
- `/ai-msdt:mockup [description]` — generate UI mockups (ASCII + Excalidraw JSON)

### Skills

- `fullstack-conventions` — naming and structure conventions

## Installation

```bash
# Add the marketplace (if not already added)
/plugin marketplace add letyshub/ai-msdt

# Install the plugin
/plugin install ai-msdt@letyshub
```

## Usage

After installation and restarting Claude Code:

```bash
# Use a command
/ai-msdt:review src/app.ts

# Agents are automatically available to Claude
```

## License

MIT
