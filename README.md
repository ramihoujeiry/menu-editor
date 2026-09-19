# TOTANGO RESTAURANT — Menu Editor

A single-page menu editor for the TOTANGO restaurant. Edit sections and items
in the sidebar, see a live A4 preview with auto-balanced three-column layout,
and print or export the result.

**Live site:** https://ramihoujeiry.github.io/menu-editor/

## Features

- **Four menus**: FOOD I, FOOD II, DRINKS I, DRINKS II (fully editable)
- **Live A4 preview** (794×1123) with sections auto-balanced across three
  columns using real rendered heights, then justified to fill the page
- **Full-height branded logo sidebar** on every printed page
- **PDF export** via the Print / Save PDF button (html2canvas + jsPDF)
- **JSON import / export** for backing up or moving menus between devices
- **Autosave** to browser localStorage, with a Reset button for factory data
- **Offline-capable**: Vue, html2canvas and jsPDF are vendored locally in
  `vendor/`, no CDN required at runtime

## Getting started

```bash
bun install   # or: npm install
bun run dev   # or: npm run dev — binds 0.0.0.0, PORT env var respected
```

Open the printed URL (defaults to http://localhost:3000).

## Build

```bash
bun run build   # or: npm run build — outputs static site to dist/
```

## Deployment

The site publishes to **GitHub Pages** from the `main` branch (legacy branch
publishing). Every push to `main` goes live at the URL above within ~10
minutes. CI (`.github/workflows/ci.yml`) validates the build on every push
and pull request.
