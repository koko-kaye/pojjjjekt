# Ćwiczenie 6. Konflikt i jak go rozwiązać

**Cel:** celowo wywołać konflikt i rozwiązać go: najpierw w przeglądarce, potem (dla chętnych) w codespace.

> [!NOTE]
> **Konflikt** oznacza, że dwie osoby zmieniły tę samą linię tego samego pliku. Git nie zgaduje, która wersja jest właściwa, i oddaje decyzję wam. To nie awaria i nic nie ginie.

## Część A. W przeglądarce, przez pull request

> [!NOTE]
> **Gałąź** to brudnopis obok głównej wersji `main`. **Pull request** to prośba o włączenie brudnopisu do `main`. Właśnie w pull requeście GitHub pozwala rozwiązać konflikt na stronie.

1. **Osoba A, na github.com:** `README.md` → ołówek → zmień pierwszą linię (tytuł z `#`) na swoją propozycję → **Commit changes…** → **Commit directly to the main branch**.
2. **Osoba B, dopiero po kroku A:** zmień tę samą linię na inny tytuł → **Commit changes…** → wybierz **Create a new branch for this commit and start a pull request**, nazwa gałęzi `tytul-b` → **Propose changes** → **Create pull request**.
3. W pull requeście pojawi się komunikat **This branch has conflicts that must be resolved**. Kliknij **Resolve conflicts**.
4. Edytor pokaże obie wersje między znacznikami:

    ```
    <<<<<<< tytul-b
    # tytuł osoby B
    =======
    # tytuł osoby A
    >>>>>>> main
    ```

5. Ustalcie wspólny tytuł. Zostawcie jedną linię albo napiszcie nową, a trzy linie ze znacznikami (`<<<<<<<`, `=======`, `>>>>>>>`) usuńcie w całości.
6. **Mark as resolved** → **Commit merge**, potem **Merge pull request** → **Confirm merge** → **Delete branch**.

✅ **Punkt kontrolny:** w `README.md` na `main` jest jeden tytuł, bez znaczników `<<<<<<<`, a pull request ma status **Merged**.

## Część B. W codespace (dla chętnych)

1. **Osoba B, na github.com:** zmień w `README.md` linię „Zespół:” i zrób commit do `main`.
2. **Osoba A, w codespace, bez wcześniejszego Sync:** zmień tę samą linię inaczej → zapisz → **Commit** → **Sync Changes**.
3. VS Code oznaczy `README.md` jako plik z konfliktem (litera **!** w Source Control). Otwórz go.
4. Nad konfliktem są przyciski: **Accept Current Change** (twoja wersja), **Accept Incoming Change** (wersja z GitHuba), **Accept Both Changes** (obie). W nowszych wersjach jest też **Resolve in Merge Editor**. Wybierz wersję albo popraw tekst ręcznie i usuń znaczniki.
5. Zapisz plik → w Source Control kliknij **+** przy pliku (albo **Complete Merge**) → **Commit** (opis jest już wpisany) → **Sync Changes**.

> [!WARNING]
> **Konflikty w notatnikach są trudniejsze.** Notatnik to w środku jeden długi plik z kodem, wynikami i numerami uruchomień. Gdy dwie osoby uruchomią ten sam notatnik, zmiany są w wielu miejscach naraz i konflikt robi się nieczytelny. Dlatego jeden notatnik ma jednego właściciela. Jeśli konflikt w notatniku jednak się zdarzy:
> 1. Naciśnij **F1** i wybierz **Merge Conflict: Accept All Incoming**, czyli wersję z GitHuba w całości (albo **Accept All Current**, czyli swoją).
> 2. Zapisz, zrób Commit i Sync.
> 3. Brakujące komórki z drugiej wersji przepisz ręcznie albo poproś prowadzącego o pomoc.
>
> Każda wcześniejsza wersja jest w historii: na github.com otwórz plik → **History**.

> [!TIP]
> **Błąd „Need to specify how to reconcile divergent branches”:** w codespace **View → Terminal**, wpisz `git config --global pull.rebase false`, naciśnij Enter i kliknij Sync jeszcze raz. W nowych codespace to ustawienie jest już włączone.

[← Ćwiczenie 5](05_commit_i_sync.md) · [Spis treści](README.md) · [Ćwiczenie 7 →](07_github_pages.md)
