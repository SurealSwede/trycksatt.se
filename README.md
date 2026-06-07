# trycksatt.se

Personlig varumärkessajt för sprinklerteknik — byggd med Jekyll på GitHub Pages.

## Komma igång lokalt

```bash
bundle install
bundle exec jekyll serve
```

Öppna sedan `http://localhost:4000`.

## Deploy till GitHub Pages

Push till `main`-branchen. GitHub Actions bygger och publicerar automatiskt.

## Struktur

- `_layouts/` — Sidmallar
- `_includes/` — Header, footer, head
- `_posts/` — Artiklar (YYYY-MM-DD-slug.md)
- `assets/css/` — Stilmall
- `verktyg/`, `artiklar/`, `om/` — Sidorna
