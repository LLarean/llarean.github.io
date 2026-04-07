---
title: Localization Char Extractor
description: Browser-based utility for extracting unique characters from localization JSON files, with Unicode range filtering, multi-language selection, and multiple output formats for font atlas generation.
language: Blazor / HTML
repo: https://github.com/LLarean/localization-char-extractor
stars: 0
---

Building a custom font atlas requires knowing exactly which characters your localization files actually use. **Localization Char Extractor** runs in the browser — drop in a localization JSON and get a clean character set, ready to feed into any font pipeline.

- Multi-language selection — process one language or all at once
- Unicode range filtering — include or exclude specific Unicode blocks
- Emoji toggle — strip or keep emoji characters from the output
- Interactive character grid — review and deselect individual characters before exporting
- Multiple output formats: plain text string and U+XXXX Unicode code point notation
- Drag-and-drop file loading, no upload required — runs entirely client-side
- localStorage persistence — selections survive a page refresh
- Keyboard shortcuts for common actions
- Expects the same JSON structure produced by [Localization Sheets Tools](https://github.com/LLarean/localization-sheets-tools)
- No installation required — open in any modern browser
- Experimental / work-in-progress
