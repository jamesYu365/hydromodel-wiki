---
title: Log
type: log
status: active
created: 2026-04-05
updated: 2026-04-14
sources: []
---

# Log

Append new entries. Do not rewrite history unless correcting an obvious factual error.

## [2026-04-05] scaffold | Initial wiki setup

Created the v1 LLM wiki structure, operating schema, templates, index, and overview pages.

## [2026-04-05] ingest | High-quality reconstruction of China's natural streamflow

Created the source page for the 2022 Miao et al. paper, added initial topic pages for natural streamflow reconstruction and China hydrology datasets, and updated the index.

## [2026-04-05] ingest | High-quality reconstruction of China's natural streamflow supplementary materials

Created a linked supplement source page, updated the main paper page with station-composition and uncertainty-analysis details, and extended the topic pages with supplementary-method context.

## [2026-04-05] ingest | CNRD v1.0

Created the source page for the 2021 CNRD v1.0 paper, updated the dataset and reconstruction topic pages to distinguish gridded runoff from routed streamflow, and extended the index.

## [2026-04-05] ingest | Satellite-based precipitation error propagation in the hydrological modeling chain across China

Created the source page for the 2024 forcing-error paper, added a topic page on precipitation-forcing error propagation, and linked its findings into the dataset and reconstruction topics.

## [2026-04-05] ingest | Warming climate and water withdrawals threaten river flow connectivity in China

Created the source page for the 2025 connectivity paper, added a topic page for river flow connectivity, and linked the paper back to the 2022 reconstruction line as a downstream application rather than a duplicate dataset artifact.

## [2026-04-05] ingest | Warming climate and water withdrawals threaten river flow connectivity in China supporting information

Created a linked supplement source page, updated the 2025 paper page with the expanded 651-station workflow and UDSBC correction details, and revised the connectivity and reconstruction topics to reflect the methodological extension.

## [2026-04-09] ingest | Model estimates of China's terrestrial water storage variation due to reservoir operation

Created the source page for the 2022 reservoir-operation and terrestrial-water-storage paper, updated the dataset and reconstruction topic pages to distinguish explicit human-managed storage modeling from natural-flow reconstruction, refreshed the index, and corrected the stale overview state note.

## [2026-04-10] maintenance | Move indexed raw source files into ingested

Moved the raw files for all sources listed in `wiki/index.md` from `raw/papers/` into `raw/papers/ingested/`, updated the affected source-page frontmatter paths, and recorded the default post-ingest move rule in `AGENTS.md`.

## [2026-04-10] ingest | Distilling hydrological and land-surface model parameters from physio-geographical properties using text-generating AI

Created the source page for the 2026 Feigl et al. paper, added a topic page on hydrological parameter regionalization to connect it with the existing `MPR`-style reconstruction sources, updated the index, and prepared the raw PDF for placement under `raw/papers/ingested/`.

## [2026-04-14] ingest | A mass-conserving-perceptron for machine-learning-based modeling of geoscientific systems

Created the source page for the 2024 `MCP` paper, added a topic page on interpretable physics-AI hydrology, updated the parameter-regionalization topic to distinguish transfer-function discovery from learnable model architecture, and updated the index for the new methodological thread.

## [2026-04-14] maintenance | Align docs with current ingest practice

Updated the ingest and raw-source docs plus the README so they reflect the current workflow: using `raw/papers/` as the active staging area, moving indexed ingested files into `raw/papers/ingested/`, and recognizing the newer interpretable physics-AI methodology thread in the repository scope.
