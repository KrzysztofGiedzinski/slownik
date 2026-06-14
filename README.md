# Słownik — Koduj z Sensem (wersja interim)

Publiczny, mobilny słownik trudnych i obcych terminów. **Wersja przejściowa** (pojedynczy plik HTML) — docelowo zastąpi ją aplikacja Astro PWA (`C:\Projekty\slownik-kodujzsensem`).

## Adres

🔗 https://krzysztofgiedzinski.github.io/slownik/ — **link-only** (`noindex`, poza wynikami Google).

## Pliki

- `slownik-terminow.html` — właściwy słownik (treść w tablicy `TERMY`, logika: szukanie, filtry, inline-linki, „głębiej", gwiazdki „znam", filtr „Ostatnie dodane", przycisk „← Wróć", zwijane filtry na telefonie).
- `index.html` — przekierowanie na słownik (czysty adres katalogu).
- `favicon.svg` — ikona (otwarta książka, paleta marki).

## Publikacja / aktualizacja

```bash
# edytuj slownik-terminow.html, potem:
git add -A && git commit -m "..." && git push
# GitHub Pages przebuduje się automatycznie (~1 min)
```

## Ważne

- **Repo jest PUBLICZNE** (wymóg darmowych GitHub Pages) — nie wstawiać tu treści poufnych (sekrety, nazwy klientów, strategie). Treść jest świadomie oczyszczona.
- Postęp nauki („gwiazdki") siedzi w `localStorage` przeglądarki — per urządzenie, nie w repo.
- Dodawanie haseł wg zasad w nagłówku komentarza tablicy `TERMY` (pola: `term, pron, cat, def, note, quote, proj`, opcjonalnie `deep`; zasada plain-first; kategorie z listy).
