---
title: SignalSystem
description: Ready-to-use event management system for Unity and .NET, based on the EventBus pattern.
language: C# / Unity / .NET
repo: https://github.com/LLarean/signal-system
stars: 0
---

Decoupling game systems is straightforward in theory and tedious in practice. **SignalSystem** is a lightweight EventBus implementation that works in both Unity and plain .NET projects.

Subscribe to signals by type, publish from anywhere, and let the bus route events without your systems needing direct references to each other. Integrated in 5+ projects as the primary inter-system communication layer.

- No MonoBehaviour dependency — works in pure C# contexts
- Type-safe signal dispatch
- Minimal setup: register, subscribe, publish
