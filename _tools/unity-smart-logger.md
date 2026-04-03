---
title: SmartLogger
description: Production-ready Unity logging system with automatic caller context, color-coded output, and ScriptableObject-based configuration.
language: C# / Unity
repo: https://github.com/LLarean/unity-smart-logger
stars: 0
---

Unity's built-in `Debug.Log` tells you what was logged but not always who logged it, especially across large codebases. **SmartLogger** wraps Unity's logging system to include automatic caller information — class name, method, line number — without requiring manual string formatting.

- Automatic caller context via `[CallerMemberName]` / `[CallerFilePath]`
- Reflection-based caching to avoid repeated type lookups
- Color-coded console output with timestamps
- ScriptableObject configuration — tweak settings without touching code
- Log level filtering: strip verbose logs from release builds
- Can be fully disabled in production with zero runtime overhead
- Used in 5+ commercial projects as a drop-in replacement for `Debug.Log`
