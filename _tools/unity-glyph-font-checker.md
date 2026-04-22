---
title: Glyph Font Checker
description: Unity editor utility that checks character coverage in TMP and Unity fonts, walks fallback chains, and warns about dynamic atlas settings that may cause missing glyphs at runtime.
language: C# / Unity
repo: https://github.com/LLarean/unity-glyph-font-checker
stars: 0
category: Unity packages
---

Localized text that looks fine in the editor can silently break at runtime when a font is missing glyphs for a particular language. **Glyph Font Checker** surfaces these problems before they ship: drag in a font, provide the text to check, and get a full breakdown of what renders and what doesn't.

Accessible via **Tools > Font Localization Checker** in the Unity editor.

- Input text directly, paste from clipboard, or load from a TextAsset
- Coverage report broken into three categories: present, fallback-covered, and missing
- Walks the full fallback font chain — shows exactly which fallback catches each character
- Reads OpenType/TrueType cmap tables directly; supports TTF, OTF, TTC, and WOFF
- Detects glyphs absent from the font file versus those simply not baked into static atlases
- Dynamic atlas capacity warnings — flags overflow risks before runtime
- Script compatibility notes for complex scripts and multi-codepoint sequences
- Requires Unity 2021.3+ and TextMeshPro
- Experimental — suitable for internal tooling and localization QA pipelines
