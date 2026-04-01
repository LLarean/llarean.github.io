---
title: "Modal Windows vs Full Screens: When to Use Each"
date: 2025-03-19
tags: [ux, game-ui]
---

When designing game UI, one of the most common structural decisions is whether to present information in a modal window or as a full screen. Both serve legitimate purposes — but using them interchangeably creates friction that players feel even when they cannot name it.

The rule I keep coming back to: **modal for context, full screen for commitment.**

## Modals interrupt — intentionally

A modal window says: "Before you continue, deal with this." That interruption is the point. Modals work well for:

- Confirmation dialogs ("Are you sure you want to spend 500 coins?")
- Short-lived notifications that require acknowledgment
- Quick parameter adjustments (volume, difficulty) that don't take the player out of their flow

The key constraint: the player should be able to process and dismiss the modal without losing their mental context. If reading the modal requires the player to forget where they were — it's the wrong pattern.

## Full screens signal transition

Full screens are appropriate when the player is moving between distinct modes of the game: the shop, the inventory, the world map, the main menu. These are not interruptions — they are destinations.

Sending a player to a full screen for a two-button confirmation dialog is noise. It communicates a weight the action does not have.

## The grey area: nested content

The most common mistake I see in shipped games is nesting a full screen's worth of content inside a modal. A modal with tabs, a scrollable list 200 items long, and sub-modals for item details is just a full screen pretending to be temporary.

When in doubt: if the player might spend more than 10–15 seconds inside it, give it a full screen.

---

*This post is a short guide originally published on LinkedIn. The original is in Russian.*
