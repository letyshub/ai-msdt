---
description: Zaprojektuj i zaimplementuj nową funkcjonalność
argument-hint: [opis-funkcjonalności]
---

# /ai-msdt:feature

## Cel
Zaprojektuj i zaimplementuj nową funkcjonalność od specyfikacji po gotowy kod.

## Instrukcje

### 1. Analiza wymagań
- Zrozum cel funkcjonalności i jej wartość biznesową
- Zidentyfikuj użytkowników i przypadki użycia
- Określ zależności z istniejącym kodem

### 2. Projekt
- Zaproponuj architekturę rozwiązania (komponenty, interfejsy, przepływ danych)
- Wskaż pliki do modyfikacji i nowe pliki do utworzenia
- Opisz kontrakt publicznego API

### 3. Implementacja
- Napisz kod zgodny z konwencjami projektu
- Zastosuj wzorce projektowe adekwatne do problemu
- Zadbaj o obsługę błędów i walidację danych wejściowych

### 4. Testy
- Napisz testy jednostkowe dla kluczowej logiki
- Uwzględnij happy path, edge cases i error handling
- Użyj wzorca AAA (Arrange-Act-Assert)

## Reguły
- Nie dodawaj kodu poza zakresem zadania
- Kod musi być bezpieczny (bez SQL injection, XSS, command injection)
- Minimalna złożoność — trzy podobne linie są lepsze niż przedwczesna abstrakcja
- Żadnych feature flags ani kompatybilności wstecznej, jeśli nie są wymagane

## Format odpowiedzi
1. **Podsumowanie** — co zostanie zbudowane i dlaczego
2. **Plan zmian** — lista plików z krótkim opisem zmian
3. **Kod** — implementacja z numerami linii
4. **Testy** — testy dla nowej funkcjonalności
