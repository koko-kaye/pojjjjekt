# Ćwiczenie 3. Uruchomienie Codespaces

**Cel:** każda osoba ma własny codespace dla repozytorium zespołu i wie, gdzie co jest.

> [!NOTE]
> **Co to jest codespace?** Komputer w chmurze GitHuba z edytorem VS Code w przeglądarce, z Pythonem i potrzebnymi bibliotekami. Każda osoba ma własny codespace, ale oba pracują na tym samym repozytorium. Codespace to biurko, repozytorium to teczka: co nie trafiło do teczki, istnieje tylko na biurku.

## Kroki (oboje)

1. W repozytorium zespołu kliknij zielony przycisk **Code** → zakładka **Codespaces** → **Create codespace on main**.
2. Jeśli GitHub zapyta o sekret `OPENAI_API_KEY`, wpisz klucz albo pomiń ten krok.
3. Poczekaj kilka minut, aż zainstalują się biblioteki. Same otworzą się pliki `README.md` i `notebooks/00_start.ipynb`.
4. Poznaj okno:
    - **lewy pasek:** Explorer (lista plików), Source Control (ikona rozgałęzienia: zmiany i Sync), czat Copilot;
    - **dolny pasek:** nazwa gałęzi `main` i ikona strzałek, czyli Sync.

> [!IMPORTANT]
> **Powrót do pracy:** wejdź na [github.com/codespaces](https://github.com/codespaces) i otwórz istniejący codespace. Nie zakładaj nowego za każdym razem.
> **Koniec pracy:** na tej samej liście ⋯ → **Stop codespace**. Codespace sam zatrzymuje się po 30 minutach bezczynności.
> **Limit:** ok. 60 godzin pracy miesięcznie na darmowym koncie, ok. 90 godzin z GitHub Education.

> [!TIP]
> **Klucz API później:** w repozytorium **Settings → Secrets and variables → Codespaces → New repository secret**, nazwa `OPENAI_API_KEY`. Potem zatrzymaj i uruchom codespace ponownie, żeby zobaczył klucz. Klucza nigdy nie wpisujemy do kodu ani do notatnika.

✅ **Punkt kontrolny:** w przeglądarce działa codespace, a po lewej widać pliki repozytorium.

[← Ćwiczenie 2](02_issues.md) · [Spis treści](README.md) · [Ćwiczenie 4 →](04_notatniki.md)
