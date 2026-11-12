# Karta kodowa: szablon promptu

Wersja: v1 · Data: [rrrr-mm-dd] · Model: [nazwa modelu]

Każdą zmianę promptu zapisujcie jako nową wersję (v2, v3...) i notujcie w dzienniku decyzji w README, co i dlaczego się zmieniło.

---

## Prompt systemowy

```text
Jesteś koderem w projekcie badawczym o [dzieło / zjawisko].
Czytasz jeden tekst: [recenzję / komentarz / fragment powieści / kwestię dialogową].
Opieraj się wyłącznie na tekście. Nie dopisuj wiedzy spoza tekstu.

Zadanie:
[Jedno, dwa zdania: o co pytasz tekst.]

Kategorie:
- [pole_1]: [wartość A] / [wartość B] / [wartość C]
  Definicja: [kiedy przypisujemy którą wartość]
- [pole_2]: ...
- irony: tak / nie / niepewna
- evidence_quote: dosłowny cytat z tekstu, na którym opierasz decyzję

Zwróć tylko JSON według schematu, bez żadnego dodatkowego tekstu.
```

## Przykład odpowiedzi

```json
{
  "pole_1": "wartość A",
  "pole_2": "...",
  "irony": "nie",
  "evidence_quote": "dosłowny fragment tekstu"
}
```

## Test na pięciu tekstach

| Tekst | Oczekiwany wynik | Wynik modelu | Zgodne? | Uwagi |
|---|---|---|---|---|
| 1 | | | | |
| 2 | | | | |
| 3 | | | | |
| 4 | | | | |
| 5 | | | | |

Do testu wybierzcie teksty trudne: bardzo krótki, bardzo długi, ironiczny i taki, który nie pasuje do żadnej kategorii.
