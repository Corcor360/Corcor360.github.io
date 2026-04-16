# Corcor360.github.io

This repository contains the Corcor360 website.

## GitHub Pages

The website is designed to function on GitHub Pages and is structured for direct hosting from this repository.

## VS Archive Manual CSV Workflow

The archive page at `vs-archive.html` loads data from `data/vs-archive/manifest.json`.

1. Add a weekly CSV file under `data/vs-archive/` (example: `2026-W15.csv`).
2. Add a manifest entry with a display label and CSV path.
3. Commit and push.

Manifest format:

```json
[
  {
    "label": "Week 15 (Apr 8-13, 2026)",
    "csv": "data/vs-archive/2026-W15.csv"
  }
]
```
