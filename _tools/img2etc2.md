---
title: img2etc2
description: Unity editor utility that automatically resizes textures to ETC2-compatible dimensions, eliminating compression artifacts on Android builds.
language: C# / Unity
repo: https://github.com/LLarean/img2etc2
image: /assets/images/img2etc2.png
stars: 9
---

ETC2 compression requires textures with dimensions divisible by 4. In practice this means artists constantly produce sprites that fail compression checks, causing visual artifacts or forcing manual resizing before each build.

**img2etc2** automates this: it hooks into Unity's asset pipeline and resizes sprite textures to ETC2-compatible dimensions, adding transparent padding where needed. Zero manual steps, no build failures from dimension mismatches.

- Rounding modes: round Up or Down to the nearest valid dimension
- Optional subfolder inclusion
- Preview of current vs. target resolution before processing
- Used internally on Android projects where ETC2/Crunch is the standard compression format
