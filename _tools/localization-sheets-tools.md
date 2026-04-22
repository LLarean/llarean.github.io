---
title: Localization Sheets Tools
description: Google Apps Script utilities for managing game localization in Google Sheets — export/import JSON, find keys, detect missing translations, and extract unique characters.
language: Google Apps Script
repo: https://github.com/LLarean/localization-sheets-tools
stars: 0
category: Localization tools
---

Managing game translations in a spreadsheet gets unwieldy fast — scattered sheets, missing keys, no easy way to sync with Unity. **Localization Sheets Tools** adds a **Localization Tools** menu directly into Google Sheets with everything needed to keep a JSON-based localization pipeline running smoothly.

- **Export JSON** — serializes all sheets into a structured localization JSON ready for Unity Localization or any JSON-driven pipeline
- **Import JSON** — parses a localization JSON and writes values back into matching cells
- **Find Key / Find Key + Duplicates** — navigates to a key by exact match; optionally reports all duplicate entries across sheets
- **Find Text** — searches for a text substring across all translation values on all sheets
- **Missing Translations** — scans all sheets and lists keys with empty cells per language
- **Sort Keys** — sorts all rows alphabetically by key across all sheets, leaving headers untouched
- **Unique Chars** — collects unique characters per language or across all sheets; useful for font atlas generation
- Installable manually via the Apps Script editor or via [clasp](https://github.com/google/clasp) for one-command updates
- No external dependencies — runs entirely within Google Apps Script
