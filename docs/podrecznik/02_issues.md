# Ćwiczenie 2. Issues: podział zadań

**Cel:** rozpisać dzisiejszą pracę na zadania i przypisać każde jednej osobie.

> [!NOTE]
> **Co to jest Issue?** Zadanie, pytanie albo zgłoszenie problemu. Ma numer (#1, #2…), osobę odpowiedzialną (**Assignee**) i miejsce na komentarze. Lista Issues to tablica zadań zespołu: od razu widać, co jest do zrobienia, kto się tym zajmuje i co już skończone.

Wszystkie Issues zakładacie w repozytorium swojego zespołu, w zakładce **Issues**. Zakłada je osoba A; osoba B w tym czasie może je czytać i komentować.

## Z czego składa się Issue

| Pole | Co wpisać |
|---|---|
| **Title** (tytuł) | krótka nazwa zadania: co i gdzie, np. „README: pola 1–2 karty projektu” |
| **Description** (opis) | co dokładnie zrobić i po czym poznać, że zadanie jest skończone |
| **Assignees** (po prawej) | osoba, która wykona zadanie |
| **Labels** (po prawej, nieobowiązkowe) | etykieta porządkująca, np. `karta projektu` albo `dane` |

Opis piszecie zwykłym tekstem. Działa tu też prosty Markdown: `- [ ]` tworzy listę do odhaczania, a zakładka **Preview** pokazuje, jak opis będzie wyglądał.

## Przykład: Issue #1 krok po kroku

1. W repozytorium zespołu kliknij zakładkę **Issues**, potem **New issue**. Nie ma zakładki? **Settings → General → Features**, zaznacz **Issues**.
2. **Title:** wpisz `README: pola 1–2 karty projektu`.
3. **Description:** wklej i dopasuj:

    ```markdown
    Uzupełnić w README.md dwa pierwsze pola karty projektu.

    - [ ] 1. Zjawisko i pytanie badawcze: jedno pytanie główne i jedno pomocnicze
    - [ ] 2. Pojęcie lub teoria: jedno pojęcie i jedno zdanie, dlaczego pasuje

    Pracuję w: codespace
    Gotowe, gdy: oba pola są wypełnione i zsynchronizowane z GitHubem.
    ```

4. Po prawej **Assignees**: wybierz osobę A.
5. Kliknij **Create**. GitHub nada zadaniu numer #1.

**Tak wygląda gotowe Issue:**

> **README: pola 1–2 karty projektu #1**
> 🟢 Open · Assignee: osoba A
>
> Uzupełnić w README.md dwa pierwsze pola karty projektu.
>
> - [ ] 1. Zjawisko i pytanie badawcze: jedno pytanie główne i jedno pomocnicze
> - [ ] 2. Pojęcie lub teoria: jedno pojęcie i jedno zdanie, dlaczego pasuje
>
> Pracuję w: codespace
> Gotowe, gdy: oba pola są wypełnione i zsynchronizowane z GitHubem.

**Co dzieje się dalej z tym Issue:**

1. Osoba A wykonuje zadanie i może odhaczać punkty listy bezpośrednio w Issue.
2. W opisie commita wpisuje `closes #1`, np. `Karta projektu: pola 1–2, closes #1` (ćwiczenie 5).
3. Po Sync GitHub sam zamknie Issue #1, a pod nim pojawi się link do commita, który je zamknął.
4. Pytania i uwagi zapisujecie w komentarzach pod Issue, żeby cały zespół je widział.

## Kolejne Issues: czym się różnią

Każde kolejne Issue zakładacie dokładnie tak samo. Zmienia się tylko tytuł, opis i osoba przypisana.

| # | Tytuł | Kto | Pracuje w | Co w opisie |
|---|---|---|---|---|
| 1 | README: pola 1–2 karty projektu | A | codespace | pola 1–2 do odhaczenia (przykład wyżej) |
| 2 | README: pola 3–4 karty projektu | B | github.com | pola 3 (źródło tekstów) i 4 (jednostka analizy) |
| 3 | Notatnik 01: pobranie próbki tekstów | A | codespace | krok 1A z notatnika `01_pobranie`; gotowe, gdy pliki są w `data/raw/` |
| 4 | Źródła: plik `data/processed/zrodla.csv` | B | github.com | 3–5 źródeł tekstów z adresem i licencją lub regulaminem |
| 5 | Strona: tytuł i pytanie w `docs/index.html` | B | github.com | tytuł projektu, pytanie badawcze, skład zespołu na stronie |

> [!TIP]
> Jeśli założycie zadania w innej kolejności, numery będą inne niż w tabeli. W kolejnych ćwiczeniach używajcie numerów, które nadał wam GitHub.

✅ **Punkt kontrolny:** w zakładce Issues jest 5 otwartych zadań, każde z przypisaną osobą i opisem z warunkiem „Gotowe, gdy”.

[← Ćwiczenie 1](01_repozytorium.md) · [Spis treści](README.md) · [Ćwiczenie 3 →](03_codespaces.md)
