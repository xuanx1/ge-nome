# Human Variation Atlas

An interactive visualization of the **1000 Genomes Project** reference cohort — an animated DNA double helix that unwinds into the raw A·T·C·G sequence, surrounded by notes that draw out what the data revealed.

Every figure is sourced from the project's own publications (1000 Genomes Project Consortium, *Nature* 2015; Byrska-Bishop et al., *Cell* 2022).

## Files

### Editable sources (`.dc.html`)
- **`Human Variation Atlas.dc.html`** — portrait layout. The helix is centered as the hero; insight cards flank it.
- **`Human Variation Atlas — Landscape.dc.html`** — landscape layout. The helix runs horizontally and unweaves in the centre, then weaves back together before leaving the frame. Includes the bottom-right typewriter "trivia" widget.

These open directly in a browser and are the files to edit. They load fonts from Google Fonts (CDN) and the local `support.js` runtime.

### Offline bundles (`offline/`)
- **`offline/Human Variation Atlas.html`**
- **`offline/Human Variation Atlas — Landscape.html`**

Fully **self-contained** — fonts, runtime, and all assets are embedded as data URIs. **No CDN or network connection required.** Open the file and it just works. These are compiled output; do not edit them directly — edit the `.dc.html` source and re-bundle.

## Features

- **Animated 3D double helix** rendered on `<canvas>` — sugar-phosphate backbones, base-pair rungs, depth shading, endless rotation/streaming.
- **Artistic / Scientific toggle** (icon toolbar) with a smooth geometry **morph** between a textured ribbon and a clean smooth model.
  - *Artistic* — strand 1 `#ee6c43`, strand 2 light grey; rungs `#f0f1f5`.
  - *Scientific* — ribbons and rungs colour-coded by variant **rarity** (rare / low-freq / common); rungs split 50-50 by their two base colours.
- **Base-pair counter** in Montserrat, conveying genome scale (~3.2 billion bp).
- **Color legend** (A/T/C/G + rarity) at bottom-left.

## Fonts

- **Space Grotesk** — headings & body
- **IBM Plex Mono** — labels, legends
- **Montserrat** — the base-pair counter

In the offline bundles these are embedded; in the `.dc.html` sources they load from Google Fonts.

## Re-bundling

After editing a `.dc.html` source, regenerate its offline bundle so the self-contained copy stays in sync. Each source contains a `<template id="__bundler_thumbnail">` used as the unpacking splash.

## Data notes

- 2,504 unrelated individuals across **26 populations** / 5 ancestry groups (phase 3); expanded to **3,202** with 698 relatives completing 602 trios at 30× (GRCh38).
- ~88M variants catalogued; ~64M are rare (<0.5%), ~12M low-frequency (0.5–5%), ~8M common (>5%).
- The 26 populations are **not** all of humanity — Middle Eastern, much of Southeast Asian, Slavic, Indigenous American, Ainu and Oceanian peoples are unsampled.
