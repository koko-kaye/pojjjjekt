# Ćwiczenie 4. Praca z notatnikami

**Cel:** uruchomić notatnik i poznać rytm pracy: prompt → kod → wynik. Osoba A zaczyna pobieranie tekstów, osoba B zbiera źródła w przeglądarce.

> [!NOTE]
> **Notatnik (.ipynb)** składa się z komórek tekstu (opis, prompt) i komórek kodu. Komórkę uruchamiasz klawiszami **Shift+Enter**, a wynik pojawia się pod nią. **Jądro (kernel)** to program, który wykonuje kod; wybierasz je raz, przy pierwszym uruchomieniu.

## Oboje: test środowiska

1. W swoim codespace otwórz `notebooks/00_start.ipynb`.
2. Kliknij w pierwszą komórkę kodu i naciśnij **Shift+Enter**. Gdy VS Code zapyta o jądro, wybierz **Python Environments → Python 3.12**.
3. Uruchamiaj komórki po kolei. Przy bibliotekach powinny być ✅. Komórka z kluczem pokaże ✅ albo ❌; bez klucza też można pracować dalej.

## Osoba A: zadanie #3

4. Otwórz `notebooks/01_pobranie.ipynb`. W komórce **Parametry** zostaw przykład („Lalka” z Wolnych Lektur) albo wpisz własne źródło.
5. **Krok 1A:** skopiuj prompt do czatu AI (Copilot Chat w Codespaces albo inny), wklej otrzymany kod do pustej komórki pod promptem i uruchom.
6. Porównaj wynik z sekcją „Po uruchomieniu powinieneś zobaczyć”. Zapisz notatnik (**Ctrl+S**, na Macu **Cmd+S**).

## Osoba B: zadanie #4, na github.com

7. W repozytorium kliknij **Add file → Create new file**. Jako nazwę wpisz `data/processed/zrodla.csv`; ukośnik sam utworzy folder.
8. Wklej nagłówek i opisz 3–5 źródeł tekstów do waszego projektu, jedno w wierszu:

    ```
    zrodlo,co_bierzemy,adres,ile_tekstow,licencja_lub_regulamin
    Wolne Lektury,„Lalka” t. I–II,https://wolnelektury.pl,2,domena publiczna
    ```

9. Kliknij **Commit changes…**, wpisz opis `Lista źródeł, closes #4`, zostaw **Commit directly to the main branch** i kliknij **Commit changes**.

> [!WARNING]
> **Notatnik ma jednego właściciela.** Gdy dwie osoby pracują równolegle w tym samym notatniku, prawie zawsze kończy się to trudnym konfliktem (ćwiczenie 6). Właściciela notatnika widać w Issue.

> [!TIP]
> Wyniki komórek zapisują się w pliku notatnika. To normalne, że po samym uruchomieniu notatnik jest oznaczony jako zmieniony.

✅ **Punkt kontrolny:** A ma wynik kroku 1A, a w `data/raw/` są pobrane pliki. B widzi `zrodla.csv` na github.com, a Issue #4 jest zamknięte.

[← Ćwiczenie 3](03_codespaces.md) · [Spis treści](README.md) · [Ćwiczenie 5 →](05_commit_i_sync.md)
