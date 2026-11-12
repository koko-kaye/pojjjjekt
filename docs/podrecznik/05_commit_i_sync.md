# Ćwiczenie 5. Commit i Sync

**Cel:** zapisać pracę w repozytorium i zobaczyć, że dwie osoby mogą edytować różne miejsca tego samego pliku bez konfliktu.

> [!NOTE]
> **Commit** to zapisana zmiana z opisem, na razie tylko w twoim codespace. **Sync** wysyła twoje commity na GitHub i pobiera zmiany innych. Zmiana jest w repozytorium dopiero po Sync.

## Gdzie to jest

- **Source Control:** ikona rozgałęzienia na lewym pasku (albo **Ctrl+Shift+G**). Lista zmienionych plików (M: zmieniony, U: nowy), pole **Message**, przycisk **Commit**, a po nim **Sync Changes**.
- **Dolny pasek:** ikona strzałek to również Sync.

## Rytm pracy (zawsze)

1. **Na początku:** Sync, żeby pobrać zmiany innych.
2. **Praca:** zapisuj pliki (**Ctrl+S**) albo włącz raz **File → Auto Save**.
3. **Na koniec:** Source Control → opis zmiany → **Commit**. Na pytanie, czy dodać wszystkie zmiany, odpowiedz **Yes** albo **Always**. Potem **Sync Changes**.
4. **Sprawdzenie:** na github.com, przy liście plików, widać twój opis commita.

## Ćwiczenie: README we dwoje

- **Osoba A, w codespace:** uzupełnij w `README.md` pola 1–2 karty projektu. Commit z opisem `Karta projektu: pola 1–2, closes #1`, potem Sync. Zrób też commit notatnika: `Krok 1A: pobranie próbki, closes #3`, i Sync.
- **Osoba B, w tym samym czasie, na github.com:** otwórz `README.md` → ikona ołówka → uzupełnij pola 3–4 → **Commit changes…**, opis `Karta projektu: pola 3–4, closes #2`, **Commit directly to the main branch**.
- **Osoba A:** jeszcze raz Sync. W codespace README ma teraz obie części.

> [!TIP]
> **Dlaczego nie było konfliktu?** Git sam łączy zmiany, jeśli dotyczą różnych miejsc w pliku. Konflikt powstaje tylko wtedy, gdy dwie osoby zmienią tę samą linię. To przećwiczycie w ćwiczeniu 6.

> [!IMPORTANT]
> **Co nie trafia do repozytorium:** folder `data/raw/` (wpisany do pliku `.gitignore`) i klucz API. Dlatego pliki z `data/raw/` nie pojawiają się w Source Control. Publikujemy tylko `data/processed/`.

✅ **Punkt kontrolny:** README na github.com ma uzupełnione pola 1–4, Issues #1–#4 są zamknięte, a w historii (link **Commits** nad listą plików) są commity obu osób.

[← Ćwiczenie 4](04_notatniki.md) · [Spis treści](README.md) · [Ćwiczenie 6 →](06_konflikt.md)
