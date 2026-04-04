---
title: Localization Key Collector
description: Unity editor utility that scans prefabs, scenes, and code to collect localization keys and export them to CSV for translation workflows.
language: C# / Unity
repo: https://github.com/LLarean/unity-localization-key-collector
stars: 0
---

Keeping localization key lists in sync with a growing project is tedious: keys appear in components on prefabs, get referenced in scenes, and get called from code — all in different places. **Localization Key Collector** scans all three sources in one pass and exports the results to CSV files ready for a translator or a localization spreadsheet.

Accessible via **Tools > Localization Key Collector** in the Unity editor.

- Scans prefabs, scenes, and code files in a single run
- Separate CSV outputs for component-based keys and code-referenced keys
- Configurable localization component name and method via project settings
- Custom CSV output paths per source type
- Requires Unity 2021.3+
- Experimental — suitable for internal tooling and custom localization setups
