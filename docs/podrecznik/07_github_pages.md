# Ćwiczenie 7. Publikacja na GitHub Pages

**Cel:** strona projektu działa pod publicznym adresem.

> [!NOTE]
> **GitHub Pages** zamienia pliki z folderu `docs/` w stronę internetową. Każdy commit w `docs/` aktualizuje stronę po minucie lub dwóch. Strona startowa to plik `docs/index.html`.

## Osoba B: zadanie #5, na github.com

1. Otwórz `docs/index.html` → ołówek.
2. Zamień `[Tytuł projektu]` (w dwóch miejscach: w `<title>` i w nagłówku) na tytuł waszego projektu. W sekcji „Pytanie badawcze” wpisz pytanie, a na dole imiona zespołu.
3. **Commit changes…**, opis `Strona: tytuł i pytanie, closes #5`, **Commit directly to the main branch**.

## Osoba A: włączenie strony

4. W repozytorium: **Settings → Pages**.
5. W sekcji **Build and deployment**: **Source: Deploy from a branch**, **Branch: main**, folder **/docs** → **Save**.
6. Po 1–2 minutach odśwież stronę ustawień. U góry pojawi się adres strony i przycisk **Visit site**.
7. Wpiszcie ten adres w `README.md`, w polu „Strona projektu”, i zróbcie commit.

> [!TIP]
> **Strona pokazuje błąd 404?** Sprawdź, czy wybrany jest folder **/docs**, i odczekaj 2 minuty. Postęp publikacji widać w zakładce **Actions**.

✅ **Punkt kontrolny:** strona zespołu działa pod adresem `nazwa-konta.github.io/nazwa-repozytorium`, a README zawiera do niej link.

[← Ćwiczenie 6](06_konflikt.md) · [Spis treści](README.md) · [Ćwiczenie 8 →](08_zgloszenie.md)
