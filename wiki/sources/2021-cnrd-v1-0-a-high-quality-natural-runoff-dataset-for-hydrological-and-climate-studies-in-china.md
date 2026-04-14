---
title: "CNRD v1.0: A high-quality natural runoff dataset for hydrological and climate studies in China"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - raw/papers/ingested/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china.pdf
---

# CNRD v1.0: A high-quality natural runoff dataset for hydrological and climate studies in China

## Summary

This paper introduces `CNRD v1.0`, a gridded natural runoff dataset for China covering 1961 to 2018 at daily, monthly, and annual time scales and `0.25°` spatial resolution. The paper positions the dataset as a public, quality-controlled hydrological product built with the VIC model and a parameter-uncertainty framework trained on 200 natural or near-natural gauge catchments.

## Key Claims

- `CNRD v1.0` is presented as the first free public gridded natural runoff dataset for China built with a comprehensive parameter-uncertainty framework.
- The dataset provides daily, monthly, and annual `0.25°` runoff estimates across China for 1961 to 2018.
- The VIC model, together with sensitivity analysis, optimization, and regionalization, can produce high-skill runoff estimates for most gauged catchments.
- Multiscale parameter regionalization provides the best regionalization solution for pseudo-ungauged and test-ungauged catchments.
- The dataset is intended for long-term hydrological and climate studies in China and as an improvement to global runoff databases.

## Methods And Evidence

- Uses the VIC land-surface model as the main reconstruction engine.
- Trains the model with 200 natural or near-natural gauge catchments.
- Uses a parameter-uncertainty workflow that combines sensitivity analysis, optimization, and regionalization.
- Emphasizes gridded runoff rather than routed streamflow at named catchment outlets.
- Frames the dataset against sparse or lower-quality Chinese and global runoff archives.

## Why It Matters

- The paper directly addresses a recurring gap in this wiki: China is poorly served by many global runoff and streamflow datasets.
- It complements the 2022 streamflow reconstruction paper by targeting runoff grids rather than monthly routed streamflow at 330 catchments.
- Because it is presented as a free public dataset, it may be more convenient for downstream comparative or applied work than datasets that are harder to obtain or less uniform.

## Tensions Or Caveats

- The abstract notes weaker calibration in arid and semiarid regions, so spatial performance is not uniform.
- The paper is about natural runoff, not identical to natural streamflow; downstream comparisons need to respect that difference.
- It uses 200 training catchments, which differs from the counts emphasized in the 2022 streamflow reconstruction materials and may reflect a different target product and workflow.

## Open Questions

- How should `CNRD v1.0` be compared against the 2022 reconstructed natural streamflow dataset: by variable, scale, training data, or use case?
- How large is the practical difference between gridded runoff and routed streamflow for the research questions in this vault?
- What are the consequences of weaker performance in arid and semiarid areas for national-scale interpretation?

## Related

- [[overview]]
- [[topics/china-hydrology-datasets]]
- [[topics/natural-streamflow-reconstruction]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]
