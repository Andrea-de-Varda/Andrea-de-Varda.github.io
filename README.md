# Andrea-de-Varda.github.io

Personal academic website, built with Jekyll and served by GitHub Pages.

## Structure

- `index.md`: home page (bio, news, selected papers). News items are edited by hand in this file; the first block is shown by default and the `Older news` block is collapsed.
- `research.md`: research overview, organized by theme.
- `publications.md`: publications page, rendered from `_data/publications.yml`.
- `_data/publications.yml`: one entry per paper. Entries are rendered in file order (newest first), grouped by `type`.
- `_layouts/default.html`: page layout, favicon, social-preview (Open Graph / Twitter) tags, and JSON-LD person schema.
- `assets/css/style.css`: all styling.
- `assets/img/favicon.svg`, `favicon-32.png`, `apple-touch-icon.png`: browser-tab icons. `assets/img/og.jpg`: social preview image.

## Publication entry fields

| Field | Meaning |
| --- | --- |
| `type` | `preprint`, `journal`, `conference`, or `chapter`; determines the section |
| `highlight` | `true` marks a selected paper (amber card; also listed on the home page) |
| `abstract` | verbatim abstract, shown behind the `Abstract` toggle |
| `award`, `note`, `media` | optional: award line, venue note (e.g. `Under review`), extra links (e.g. MIT News) |
| `id` | optional anchor (e.g. `cost-of-thinking`) |
| `exchange` | optional list of letters and replies rendered inside the main paper's card |
| `reply` | `true` for PNAS replies, which are kept in the data file but rendered only inside the `exchange` block |

## Building locally

GitHub Pages builds the site on push. To preview locally, install Jekyll and run:

```
jekyll build -d /tmp/_site && (cd /tmp/_site && python3 -m http.server 8765)
```

Assets use absolute paths, so preview over HTTP rather than opening the HTML files directly.
