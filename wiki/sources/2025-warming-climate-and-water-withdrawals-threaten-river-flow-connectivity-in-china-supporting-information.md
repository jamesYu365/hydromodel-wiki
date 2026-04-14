---
title: "Warming climate and water withdrawals threaten river flow connectivity in China supporting information"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information.pdf"
---

# Warming climate and water withdrawals threaten river flow connectivity in China supporting information

## Summary

The supporting information makes the 2025 connectivity paper methodologically legible. It shows that the paper reuses the natural-streamflow reconstruction lineage, but extends it with a larger 651-station calibration/validation base, an upstream-downstream scaled bias-correction (`UDSBC`) procedure, low-flow-focused evaluation metrics, and a modified dendritic connectivity index (`DCI`) that treats zero-flow fragments as temporary barriers.

## Key Additions

- Re-states the water-balance naturalization logic used to reconstruct natural streamflow from measured gauge discharge and direct water-abstraction terms.
- Expands the calibration/validation basis to `651` hydrological stations: `342` daily stations and `309` monthly stations during `1961–1979`.
- Specifies station-screening criteria, including naturalized records, minimal upstream regulation, pre-1980 coverage, hydrographs without clear artificial regulation, and limited missingness.
- Introduces `UDSBC`, a statistical post-processing and bias-correction workflow that propagates gauge information through gauged, upstream, nested, and ungauged river classes.
- Defines low-flow-oriented model evaluation using `LogCC`, `LogNSE`, `Pbias`, and `LogKGE`, explicitly to better represent intermittence.
- Defines the modified `DCI` used for connectivity analysis, where zero-flow channel fragments act as temporary barriers.

## Why It Matters

- The supplement answers the main “update or reuse?” question: the 2025 paper is not just a rerun of the 2022 setup, but a materially extended modeling chain aimed at intermittency and connectivity.
- It shows that low-flow representation is a first-class modeling objective here, not a side effect.
- It also surfaces an important methodological bridge from hydrological reconstruction to ecological network metrics.

## Tensions Or Caveats

- The 2025 results inherit not only reconstruction assumptions but also a substantial post-processing layer through `UDSBC`.
- Because low-flow metrics and bias correction are emphasized, comparisons to earlier papers based on more conventional monthly skill summaries should be done carefully.
- The larger station base improves scope, but also means the 2025 workflow is no longer directly interchangeable with the 2022 setup.

## Open Questions

- How much of the 2025 connectivity result depends on `UDSBC` rather than on the raw hydrological simulation itself?
- Which parts of the 651-station workflow are directly comparable to the earlier 330-station and 200-station workflows?
- How sensitive is the modified `DCI` to river-network discretization and zero-flow threshold assumptions?

## Related

- [[overview]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[topics/river-flow-connectivity]]
- [[topics/natural-streamflow-reconstruction]]
