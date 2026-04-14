---
title: "High-quality reconstruction of China's natural streamflow"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2022-high-quality-reconstruction-of-chinas-natural-streamflow.pdf"
  - "[[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]"
---

# High-quality reconstruction of China's natural streamflow

## Summary

This paper presents a gauge-based reconstruction of monthly natural streamflow across 330 Chinese catchments from 1961 to 2018. The core contribution is not just a new dataset, but a reconstruction scheme that combines a VIC land-surface model, a Lohmann routing model, manual flow-direction correction, and a parameter-uncertainty workflow designed to reduce bias against natural or near-natural gauges.

## Key Claims

- The study reconstructs what it describes as the first high-quality gauge-based natural streamflow dataset covering 330 Chinese catchments from 1961 to 2018.
- Flow-direction correction materially improves the match between upstream routing cells and observed drainage areas.
- A parameter-uncertainty workflow built from sensitivity analysis, optimization, and regionalization reduces bias between modeled and inferred natural streamflow.
- The resulting monthly streamflow reconstruction performs strongly at national scale, with about 83% of catchments reporting `NSE > 0.7` and about 56% reporting `KGE > 0.7`.
- The resulting low-bias dataset is intended to support water-resources assessment, allocation, and climate-impact analysis in China.

## Methods And Evidence

- Uses the VIC macroscale land-surface model coupled with the Lohmann routing model.
- Uses meteorological forcing, land-surface inputs, corrected routing networks, and monthly natural or near-natural records from 330 gauge stations.
- Trains and validates the model against inferred natural or near-natural gauge records, with a 230-station training subset and a 100-station test subset.
- Treats routing-network correction as a prerequisite for calibration because gauge location, drainage area, and upstream flow direction strongly affect routed streamflow.
- Uses a parameter-uncertainty framework to identify sensitive parameters, optimize them, and regionalize them to ungauged areas.
- The supplement clarifies that the 330 stations include 149 Type-1 naturalized records, 122 Type-2 no-upstream-dam records, and 59 Type-3 records with upstream dam influence but still treated as near-natural enough for reconstruction.
- The supplement also spells out the uncertainty workflow as four sensitivity-analysis methods (`SOT`, `MARS`, `DT`, `Sobol`), followed by `ASMO` optimization and `MPR` regionalization.

## Why It Matters

- China has major water-scarcity and river-regulation pressures, so observed streamflow often reflects human intervention rather than natural hydrological behavior.
- A long-term naturalized streamflow dataset is useful for separating climate-driven change from direct human water management effects.
- The reconstruction scheme is also presented as a transferable approach for other regions facing sparse or distorted natural-flow observations.
- Later work in this wiki uses this modeling line for downstream applications such as national river-flow-connectivity analysis, not just for building a dataset.

## Tensions Or Caveats

- The reconstruction depends on inferred natural or near-natural gauge records, so its quality still rests partly on upstream judgment about which stations are sufficiently naturalized.
- The paper emphasizes high skill for monthly streamflow, so care is needed before assuming equivalent quality at other temporal resolutions or for all downstream uses.
- The method includes substantial manual routing correction and regional parameter treatment, which may make exact reproduction or extension operationally nontrivial.
- The supplementary materials introduce a training-count ambiguity: the main paper describes 230 training stations and 100 test stations, while the supplement mentions optimization at 200 training stations.

## Open Questions

- How does dataset quality vary across the 10 Chinese water-resources regions rather than only in national aggregate?
- Which hydrological regimes or basin types still show weak reconstruction skill after calibration?
- How should this dataset be compared with later products such as `CNRD v1.0` in terms of coverage, resolution, and intended use?
- What explains the training-station count discrepancy between the main paper and the supplementary materials?

## Related

- [[overview]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]]
- [[topics/natural-streamflow-reconstruction]]
- [[topics/china-hydrology-datasets]]
