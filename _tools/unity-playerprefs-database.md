---
title: PlayerPrefsDatabase
description: Zero-dependency save system for Unity — typed read/write over PlayerPrefs with JSON serialization, in a single line of code.
language: C# / Unity
repo: https://github.com/LLarean/unity-playerprefs-database
stars: 0
---

A minimal save system for small-to-medium Unity games that don't need a full database but want more structure than raw PlayerPrefs key strings.

**PlayerPrefsDatabase** stores any serializable data as JSON under a single PlayerPrefs key per "table". The API is deliberately minimal:

```csharp
Database.Save("settings", data);
var data = Database.Load<SettingsData>("settings");
```

- Zero external dependencies
- Works with any serializable type
- Suitable for save data, settings, and player progress in mobile games, prototypes, and game jams
