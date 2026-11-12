# Podręcznik laboratorium: GitHub w praktyce

Po dzisiejszych zajęciach wasz zespół ma własne repozytorium z szablonu, zadania rozpisane w Issues, działający Codespace, kartę projektu w README, stronę na GitHub Pages i zgłoszenie u prowadzącego. Wszystko robimy w przeglądarce, na GitHubie.

> [!NOTE]
> **Role w parze.** Osoba A pracuje głównie w Codespaces, osoba B głównie na stronie github.com. Pracujesz sam? Wcielasz się w obie role: jako A pracujesz w codespace, jako B w drugiej karcie przeglądarki.

## Plan zajęć

| # | Ćwiczenie | Kto | Czas |
|---|---|---|---|
| 1 | [Repozytorium z szablonu](01_repozytorium.md) | A, potem B | 10 min |
| 2 | [Issues: podział zadań](02_issues.md) | A | 10 min |
| 3 | [Uruchomienie Codespaces](03_codespaces.md) | oboje | 10 min |
| 4 | [Praca z notatnikami](04_notatniki.md) | A: notatnik, B: źródła | 15 min |
| 5 | [Commit i Sync](05_commit_i_sync.md) | oboje | 15 min |
| 6 | [Konflikt i jak go rozwiązać](06_konflikt.md) | oboje | 15 min |
| 7 | [Publikacja na GitHub Pages](07_github_pages.md) | B, potem A | 10 min |
| 8 | [Zgłoszenie u prowadzącego](08_zgloszenie.md) | jedna osoba | 5 min |

## Zasady współpracy

1. **Przed pracą Sync, po pracy Commit i Sync.** Wtedy konflikty zdarzają się rzadko.
2. **Każde zadanie to jedno Issue z jedną osobą odpowiedzialną.**
3. **Jeden plik edytuje naraz jedna osoba.** Notatnik ma zawsze jednego właściciela.
4. **Małe commity z opisem.** Fraza `closes #numer` w opisie zamyka zadanie.
5. **Klucze API i surowe dane nigdy nie trafiają do repozytorium.**

## Słowniczek

| Pojęcie | Co to jest | Porównanie |
|---|---|---|
| Repozytorium | folder projektu z całą historią zmian | teczka projektu |
| Szablon | repozytorium, z którego robi się niezależne kopie | czysty formularz |
| Issue | zadanie lub pytanie z osobą odpowiedzialną i dyskusją | karteczka na tablicy zadań |
| Codespace | komputer w chmurze z edytorem w przeglądarce | wynajęte biurko |
| Notatnik (.ipynb) | plik z komórkami tekstu i kodu oraz ich wynikami | zeszyt laboratoryjny |
| Jądro (kernel) | program, który wykonuje kod z komórek notatnika | silnik notatnika |
| Commit | zapisana zmiana z opisem, autorem i datą | wpis do dziennika |
| Sync | wysłanie swoich commitów na GitHub i pobranie cudzych | wymiana z teczką |
| Gałąź (branch) | osobna linia zmian obok głównej wersji `main` | brudnopis obok czystopisu |
| Pull request | prośba o włączenie zmian z gałęzi do `main` | wniosek o wklejenie poprawek |
| Konflikt | dwie osoby zmieniły to samo miejsce w pliku | dwie poprawki w jednym zdaniu |
| GitHub Pages | strona internetowa zbudowana z plików w repozytorium | witryna projektu |
| Sekret | zaszyfrowana wartość, np. klucz API, dostępna w codespace | sejf |

## Linki

- Prezentacja z zajęć: [„Lalka” 1887–2026: projekt od podstaw](https://claude.ai/artifact/ThG9USc6EBTba2iqBGSgz8)
- Szablon: [github.com/alblesniak/szablon-projektu](https://github.com/alblesniak/szablon-projektu)
- Zgłoszenia projektów: [Issues w repozytorium szablonu](https://github.com/alblesniak/szablon-projektu/issues)
