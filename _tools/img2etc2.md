---
title: img2etc2
description: Automatically resize Unity images for optimal ETC2/Crunch compression.
language: C# / Unity
repo: https://github.com/LLarean/img2etc2
stars: 9
---

ETC2 compression requires textures with dimensions divisible by 4. In practice this means artists constantly produce sprites that fail compression checks, causing visual artifacts or forcing manual resizing before each build.

**img2etc2** automates this: it hooks into Unity's asset pipeline and resizes sprite textures to the nearest ETC2-compatible dimensions automatically. Zero manual steps, no build failures from dimension mismatches.

Used internally on projects targeting Android where ETC2/Crunch is the standard compression format.
