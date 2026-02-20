# AI-MSDT (Multi-Stack Development Toolkit)

Plugin do Claude Code CLI z agentami i narzędziami dla fullstack developera.

## Stack

- .NET / C#
- React / Angular / Vue
- TypeScript
- Go
- Python

## Zawartość

### Agenty (12)

| Agent | Opis |
|-------|------|
| `architect` | Architekt systemu |
| `api-designer` | Projektant API (REST/gRPC) |
| `code-reviewer` | Code reviewer |
| `refactor-advisor` | Doradca refaktoryzacji |
| `test-engineer` | Inżynier testów |
| `security-auditor` | Audytor bezpieczeństwa |
| `db-architect` | Architekt baz danych |
| `devops-engineer` | Inżynier DevOps |
| `docs-writer` | Technical writer |
| `debugger` | Debugger / diagnostyk |
| `performance-tuner` | Specjalista od wydajności |
| `ux-consultant` | Konsultant UX |

### Komendy

- `/review [plik]` — code review
- `/explain [plik]` — wyjaśnienie kodu
- `/test [plik]` — generowanie testów

### Skille

- `fullstack-conventions` — konwencje nazewnictwa i struktury

## Instalacja

```bash
# Dodaj marketplace (jeśli nie masz)
/plugin marketplace add letyshub/ai-msdt

# Zainstaluj plugin
/plugin install ai-msdt@letyshub
```

## Użycie

Po instalacji i restarcie Claude Code:

```bash
# Użyj komendy
/ai-msdt:review src/app.ts

# Agenty są dostępne automatycznie dla Claude
```

## Licencja

MIT
