# Corcor360.github.io

This repository contains the Corcor360 website.

## Localization

The site now supports three languages:

- English (default): `en/`
- Spanish: `es/`
- Portuguese: `pt/`

Root pages (`index.html`, `PPLE-Home.html`, `train-tracker.html`, `vs-tracker.html`, `vs-archive.html`) redirect to the English versions under `en/`.

## GitHub Pages

The website is designed to function on GitHub Pages and is structured for direct hosting from this repository.

## Train Tracker

The train tracker page at `train-tracker.html` loads data from this published Google Sheets CSV URL:

`https://docs.google.com/spreadsheets/d/e/2PACX-1vQU6Du4tIuOoUGSLdggDJE1cA00Hs_Ujj1XcmSIklAEJyYLBFCYlreSW0ccCLSc6yN_r3WCB1FFSP9z/pub?output=csv`

Expected CSV columns:

- `Date`
- `Conductor`
- `VIP`

## VS Archive Manual CSV Workflow

Archive pages (`en/vs-archive.html` and `es/vs-archive.html`) load data from `data/vs-archive/manifest.json`.

1. Add a weekly CSV file under `data/vs-archive/` (example: `2026-W15.csv`).
2. Add a manifest entry with localized labels and the CSV filename.
3. Commit and push.

Manifest format:

```json
[
  {
    "labels": {
      "en": "Week 15 (Apr 8-13, 2026)",
      "es": "Semana 15 (8-13 abr 2026)"
    },
    "csv": "2026-W15.csv"
  }
]
```
