---
name: fullstack-conventions
description: Konwencje i wzorce dla projektów fullstack (.NET, React, Angular, Go, TS, Python)
globs: ["**/*.cs", "**/*.ts", "**/*.tsx", "**/*.vue", "**/*.go", "**/*.py", "**/*.jsx"]
---

# Konwencje Fullstack

## Struktura projektu
- Oddzielaj warstwy: transport → logika biznesowa → dane
- Feature-based structure dla frontendów
- Clean Architecture dla .NET

## Nazewnictwo
- **Klasy/typy**: PascalCase
- **Funkcje/metody**: camelCase (TS/Go), snake_case (Python), PascalCase (.NET)
- **Zmienne**: camelCase (TS/Go/.NET), snake_case (Python)
- **Stałe**: SCREAMING_SNAKE_CASE
- **Pliki komponentów**: PascalCase (React/Angular/Vue)

## Error handling
- Używaj Result pattern zamiast exceptions gdzie możliwe
- Loguj z kontekstem (correlation ID, user ID)
- Nie ukrywaj błędów — propaguj do warstwy wyżej

## API
- RESTful: rzeczowniki, HTTP verbs, poprawne status codes
- Zawsze pagination dla list
- Wersjonowanie przez URL path

## Testy
- AAA pattern (Arrange-Act-Assert)
- Nazwy opisują zachowanie
- 70% unit / 20% integration / 10% E2E

## Git
- Conventional commits: feat/fix/refactor/docs/test/chore
- Małe, atomowe commity
- Branch per feature
