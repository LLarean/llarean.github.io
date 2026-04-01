---
title: "UI Image Optimization in Unity: Formats, Sizes, and Compression"
date: 2025-04-01
tags: [unity, optimization, ui]
---

Texture memory is one of the most common sources of performance problems in mobile Unity projects — and UI textures are often the biggest offenders, precisely because they are treated as an afterthought.

Here is what I have learned optimizing UI atlases across several commercial projects.

## ETC2 is your baseline on Android

For Android builds, ETC2 should be the default compression for UI sprites. It gives a good quality-to-size ratio and is hardware-accelerated on all modern Android GPUs. The catch: ETC2 requires textures with dimensions that are multiples of 4 — and for best results, powers of 2.

This is the problem that [img2etc2](https://github.com/LLarean/img2etc2) solves. It automatically resizes sprites to ETC2-compatible dimensions before the build step, so artists don't have to think about it.

## Atlas packing matters more than individual texture settings

A single unatlased UI sprite generates a draw call. Pack 50 sprites into one atlas and you get one draw call for all of them. Unity's Sprite Atlas system handles this, but it requires deliberate organization:

- Group sprites by screen / usage context, not by visual category
- Keep sprites that appear together in the same atlas
- Don't put rarely-used sprites in a hot atlas

## Mipmaps: off for UI

UI textures are rendered at a fixed pixel size on screen — they don't benefit from mipmapping, and enabling it wastes 33% additional memory. Make sure `Generate Mip Maps` is unchecked for all UI texture imports.

## Readable textures: also off

`Read/Write Enabled` keeps a CPU-side copy of the texture in RAM. You almost never need this for UI sprites. Leaving it on doubles the memory footprint of the texture.

---

*Originally published as a LinkedIn guide. The original is in Russian.*
