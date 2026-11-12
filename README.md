# [Tytuł projektu]

**Zespół:** [imię i nazwisko], [imię i nazwisko]
**Zajęcia:** Nowa humanistyka, kulturoznawstwo, studia magisterskie
**Strona projektu:** [adres z GitHub Pages, np. https://nazwa-konta.github.io/nazwa-repozytorium/]

> [!NOTE]
> **Na laboratorium:** instrukcje krok po kroku są w [podręczniku laboratorium](docs/podrecznik/README.md).
> Prezentacja z zajęć: [„Lalka” 1887–2026: projekt od podstaw](https://claude.ai/artifact/ThG9USc6EBTba2iqBGSgz8).
> Zgłoszenia projektów: [Issues w repozytorium szablonu](https://github.com/alblesniak/szablon-projektu/issues).

---

## Karta projektu

Wypełniajcie kartę na bieżąco. Pola 1–4 przygotowujecie na start, resztę uzupełniacie w trakcie pracy.

### 1. Zjawisko i pytanie badawcze
*O co pytam?*

[Wpisz jedno główne pytanie badawcze i jedno lub dwa pytania pomocnicze.]

### 2. Pojęcie lub teoria
*Co oświetli wynik?*

[Np. horyzont oczekiwań, wspólnoty interpretacyjne, kapitał kulturowy, ramowanie, teoria adaptacji.]

### 3. Źródło tekstów
*Skąd, ile i czy wolno pobrać?*

| Źródło | Co z niego bierzemy | Ile tekstów | Regulamin / prawo sprawdzone? |
|---|---|---|---|
| [np. Wolne Lektury] | [tekst powieści] | [1] | [tak, domena publiczna] |
| | | | |

### 4. Jednostka analizy
*Cały tekst czy fragment?*

[Np. scena, rozdział, akapit, komentarz, recenzja.]

### 5. Karta kodowa
*Pola, kategorie, definicje.*

| Pole | Wartości | Definicja |
|---|---|---|
| [np. blame] | [Wokulski / Izabela / obie strony / społeczeństwo / brak] | [komu tekst przypisuje winę] |
| evidence_quote | dosłowny cytat | fragment, na którym model oparł decyzję |

### 6. Walidacja
*Ile tekstów sprawdzę ręcznie?*

[Np. losowa próba 50 tekstów kodowana ręcznie bez patrzenia na wynik modelu; procent zgodności i kappa Cohena.]

### 7. Wizualizacja
*Jaki wykres odpowie na pytanie?*

[Jeden wykres, jedno pytanie.]

### 8. Analiza i porównania
*Z czym porównam? Co policzę zwykłym liczeniem słów?*

[Np. epoki, wersje, postaci; Korpusomat.]

### 9. Etyka i prawo
*Dane osobowe, prawa autorskie, wybór modelu.*

[Np. pseudonimizacja nicków, krótkie cytaty na stronie, surowe dane poza repozytorium.]

### 10. Czego ten projekt nie powie?

[Granice: kogo nie obejmują dane, czego nie widzi metoda.]

---

## Dziennik decyzji

Zapisujcie tu każdą decyzję, która wpływa na wynik: definicję sceny, sposób łączenia imion postaci, wersję modelu, datę pobrania danych.

| Data | Decyzja | Dlaczego |
|---|---|---|
| [rrrr-mm-dd] | [np. rozdział powieści liczymy jako jedną scenę] | [w powieści nie ma scen jak w scenariuszu] |

---

## Struktura repozytorium

```
README.md               karta projektu i dziennik decyzji (ten plik)
notebooks/
  00_start.ipynb        test środowiska: biblioteki i klucz API
  01_pobranie.ipynb     pobranie tekstów i metadanych
  02_przetwarzanie      (dodacie sami) sieć, role, kodowanie przez LLM
  03_wizualizacja       (dodacie sami) wykresy i grafy
data/
  raw/                  surowe dane: NIE trafiają do repozytorium (.gitignore)
  processed/            tabele po pseudonimizacji i wyniki: publikujemy
prompts/                prompty i karta kodowa w wersjach
docs/index.html         strona projektu (GitHub Pages)
docs/podrecznik/        podręcznik laboratorium: ćwiczenia krok po kroku
.devcontainer/          przepis na środowisko Codespaces
requirements.txt        lista bibliotek Pythona
```

---

## Jak pracować

1. **Start:** zielony przycisk **Code** → zakładka **Codespaces** → **Create codespace on main**. Pierwsze uruchomienie trwa kilka minut, bo instalują się biblioteki.
2. **Powrót do pracy:** wchodzisz na [github.com/codespaces](https://github.com/codespaces) i otwierasz istniejący codespace. Nie zakładaj nowego za każdym razem.
3. **Zapis pracy:** ikona **Source Control** po lewej → opis zmiany → **Commit** → **Sync Changes**. Codespace to biurko, repozytorium to teczka: co nie zostało zapisane commitem i zsynchronizowane, nie istnieje w repozytorium.
4. **Praca w zespole:** przed pracą zrób **Sync**, żeby pobrać zmiany innych. Jeden plik edytuje naraz jedna osoba.
5. **Koniec pracy:** zatrzymaj codespace (lista na github.com/codespaces → **Stop codespace**). Sam zatrzyma się po 30 minutach bezczynności.

### Klucz API

Klucza nigdy nie wpisujemy do kodu ani do notatnika. Przy tworzeniu codespace GitHub zapyta o sekret `OPENAI_API_KEY`. Można go też dodać później: **Settings → Secrets and variables → Codespaces → New repository secret**. Po dodaniu sekretu codespace trzeba uruchomić ponownie.

### Strona projektu

**Settings → Pages → Source: Deploy from a branch → Branch: main, folder /docs → Save.** Adres pojawi się po minucie lub dwóch. Stronę edytujecie w pliku `docs/index.html`.
