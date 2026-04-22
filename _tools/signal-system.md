---
title: SignalSystem
description: Lightweight EventBus for Unity and .NET — type-safe signal dispatch with automatic subscriber detection, originally built at Owlcat Games.
language: C# / Unity / .NET
repo: https://github.com/LLarean/signal-system
stars: 0
category: C# / .NET
---

Decoupling game systems is straightforward in theory and tedious in practice. **SignalSystem** is an EventBus implementation originally created at Owlcat Games, adapted for open use in Unity and plain .NET projects.

Subscribe to signals by type, publish from anywhere, and let the bus route events without your systems needing direct references to each other.

- No MonoBehaviour dependency — works in pure C# contexts
- Automatic subscriber detection — no manual registration boilerplate
- Reflection-based caching for repeated lookups
- Null-safe handling — missing subscribers don't throw
- NUnit test suite included
- Integrated in 5+ projects as the primary inter-system communication layer
