---
title: SmartLogger
description: Enhanced Unity logging utility with automatic caller information and performance optimization.
language: C# / Unity
repo: https://github.com/LLarean/unity-smart-logger
stars: 0
---

Unity's built-in `Debug.Log` tells you what was logged but not always who logged it, especially across large codebases. **SmartLogger** wraps Unity's logging system to include automatic caller information — class name, method, line number — without requiring manual string formatting.

Features:
- Automatic caller context via `[CallerMemberName]` / `[CallerFilePath]`
- Log level filtering (strip verbose logs from release builds)
- Color-coded output in the Unity console
- Used in 5+ commercial projects as a drop-in replacement for `Debug.Log`
