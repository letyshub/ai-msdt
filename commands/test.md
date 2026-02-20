---
description: Napisz testy dla wskazanego kodu
argument-hint: [sciezka-do-pliku]
---

# /test

## Cel
Napisz testy jednostkowe dla wskazanego kodu.

## Instrukcje
1. Zidentyfikuj publiczne API do przetestowania
2. Określ edge case'y i warunki brzegowe
3. Napisz testy w odpowiednim frameworku dla stacku
4. Użyj wzorca AAA (Arrange-Act-Assert)

## Reguły
- Nazwy testów opisują zachowanie: `Should_DoSomething_When_Condition`
- Jeden powód do faila na test
- Uwzględnij: happy path, edge cases, error handling
