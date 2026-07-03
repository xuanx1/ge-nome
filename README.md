# Human Variation Atlas

A [visualisation](https://xuanx1.github.io/ge-nome/) of the **1000 Genomes Project** reference cohort — an animated DNA double helix that unwinds into the raw A·T·C·G sequence, surrounded by notes that draw out what the data revealed.

Every figure is sourced from the project's own publications (1000 Genomes Project Consortium, *Nature* 2015; Byrska-Bishop et al., *Cell* 2022).


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


## Data

- 2,504 unrelated individuals across **26 populations** / 5 ancestry groups (phase 3); expanded to **3,202** with 698 relatives completing 602 trios at 30× (GRCh38).
- ~88M variants catalogued; ~64M are rare (<0.5%), ~12M low-frequency (0.5–5%), ~8M common (>5%).
- The 26 populations are **not** all of humanity — Middle Eastern, much of Southeast Asian, Slavic, Indigenous American, Ainu and Oceanian peoples are unsampled.
