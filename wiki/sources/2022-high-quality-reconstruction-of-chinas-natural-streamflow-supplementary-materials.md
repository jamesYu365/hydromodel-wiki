---
title: "High-quality reconstruction of China's natural streamflow supplementary materials"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials.docx"
---

# High-quality reconstruction of China's natural streamflow supplementary materials

## Summary

The supplementary materials make the main paper much more operational. They spell out how naturalized streamflow is constructed from observed gauge discharge, how the 330 stations are divided by record type, and how the parameter-uncertainty workflow is implemented through sensitivity analysis, optimization, and multiscale parameter regionalization.

## Key Additions

- Defines the water-balance principle used to convert measured gauge discharge into naturalized streamflow by adding back human-altered water volumes such as irrigation withdrawals, industrial and domestic use, diversions, flood-protection flows, and reservoir storage effects.
- Clarifies the composition of the 330-station dataset: 149 Type-1 naturalized records, 122 Type-2 records without upstream dams, and 59 Type-3 records with upstream dams but still treated as near-natural enough for reconstruction.
- Details the parameter-uncertainty workflow with four sensitivity-analysis methods: `SOT`, `MARS`, `DT`, and metamodel-based `Sobol`.
- Describes optimization through adaptive surrogate modeling-based optimization (`ASMO`) and parameter transfer through multiscale parameter regionalization (`MPR`).
- Lists supplementary tables and figures that support claims about gauge quality, routing, calibrated parameters, skill metrics, and post-processing.

## Why It Matters

- The supplement is where the paper becomes auditable: it shows what counts as a usable station, what kinds of human interference were adjusted, and how parameter tuning was actually operationalized.
- It strengthens confidence in the dataset by explaining the station-quality logic instead of leaving “natural or near-natural” as a vague label.
- It also surfaces implementation complexity that is easy to miss in the main paper.

## Tensions Or Caveats

- The supplement describes the 330-station record set as partly naturalized and partly near-natural, which reinforces that “natural” here is reconstructed or inferred rather than directly observed.
- It introduces a possible counting ambiguity around model training, since the supplement mentions parameter tuning at 200 training stations while the main paper describes a 230-station training subset and a 100-station test subset.
- The method remains operationally heavy: manual routing correction, station screening, uncertainty analysis, optimization, and regionalization all matter.

## Open Questions

- Why does the supplement mention 200 training stations while the main text refers to 230 training stations?
- How sensitive are the final reconstructions to the inclusion of Type-3 stations with upstream dam influence?
- What practical effect did the statistical post-processing step have on basin-level performance beyond the summary metrics?

## Related

- [[overview]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[topics/natural-streamflow-reconstruction]]
- [[topics/china-hydrology-datasets]]
