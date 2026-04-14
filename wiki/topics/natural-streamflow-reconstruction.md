---
title: "Natural Streamflow Reconstruction"
type: topic
status: active
created: 2026-04-05
updated: 2026-04-05
sources:
  - "[[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]]"
  - "[[sources/2022-model-estimates-of-chinas-terrestrial-water-storage-variation-due-to-reservoir-operation]]"
  - "[[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]"
  - "[[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]"
  - "[[sources/2024-satellite-based-precipitation-error-propagation-in-the-hydrological-modeling-chain-across-china]]"
  - "[[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]]"
  - "[[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]"
---

# Natural Streamflow Reconstruction

## Summary

Natural streamflow reconstruction is the task of estimating how rivers would have flowed without major direct human interventions such as dams, diversions, withdrawals, or reservoir operations. In this wiki, it matters because much observed streamflow in China reflects water management as well as climate and catchment behavior.

## Key Points

- Naturalized flow records are needed when observed flow is too distorted by human activity to represent the underlying hydrological regime.
- Simple reconstruction approaches such as water-balance or regression methods can struggle in strongly disturbed basins or in areas with sparse observations.
- The 2022 Miao et al. paper treats routing correction and parameter-uncertainty analysis as critical components of credible reconstruction, not as secondary details.
- Its supplementary materials clarify that the usable station pool mixes naturalized, no-upstream-dam, and low-dam-influence records rather than relying on one uniform record type.
- `CNRD v1.0` shows a closely related but distinct path: model natural runoff on a gridded field first, then use that as a reusable national-scale dataset.
- The 2022 reservoir-operation paper is a useful boundary case for this topic because it models anthropogenic storage explicitly rather than trying to remove human influence to recover natural flow.
- The 2024 precipitation-error study highlights that forcing uncertainty can be damped by routing or amplified in dry, small, water-limited catchments, which matters when judging reconstructed hydrological products.
- The 2025 river-flow-connectivity paper shows how reconstructed natural-flow modeling can be extended into a large-scale application layer for ecological and water-withdrawal analysis.
- Its supporting information shows that this extension is methodologically substantial: larger station coverage, bias correction, low-flow-focused metrics, and a modified connectivity index.
- Monthly natural streamflow datasets are especially useful for climate-impact analysis, water-resources assessment, and model calibration.

## Evidence Base

- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]] argues that China needs reconstructed natural flow because gauge records are heavily affected by dams, diversions, irrigation, and other anthropogenic influences.
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]] details the station-quality logic and the actual uncertainty-analysis pipeline used to operationalize reconstruction.
- [[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]] extends the picture by showing how a runoff-focused gridded product can be built from a similar uncertainty-analysis philosophy.
- [[sources/2022-model-estimates-of-chinas-terrestrial-water-storage-variation-due-to-reservoir-operation]] helps clarify the conceptual boundary between naturalization-oriented reconstruction and explicit human-water-management modeling.
- [[sources/2024-satellite-based-precipitation-error-propagation-in-the-hydrological-modeling-chain-across-china]] adds evidence that forcing-error behavior differs between runoff and streamflow stages, so evaluation targets matter.
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]] shows a downstream use of reconstructed natural flow: estimating intermittency and connectivity shifts across a national river network.
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]] clarifies that the 2025 workflow is not identical to the 2022 setup and adds a distinct correction and evaluation layer.

## Open Questions

- What are the practical differences between reconstructed natural streamflow, naturalized gauge records, and near-natural observed records in later datasets?
- When should this wiki prefer runoff products like `CNRD v1.0` over reconstructed streamflow products, and when should it not?
- Which reconstruction choices most affect downstream interpretation: training gauges, routing correction, or parameter regionalization?
- How much does routing-induced damping of forcing error contribute to the apparent skill of reconstructed streamflow products?
- How much do results depend on mixing Type-1 naturalized records with Type-2 and Type-3 near-natural observations?
- Which modeling assumptions become most consequential when reconstructed flow is used for ecological connectivity claims rather than hydrological fit metrics?
- How comparable are 2022 and 2025 skill claims once low-flow log metrics and `UDSBC` bias correction are introduced?
- How should this wiki connect natural-flow reconstruction to explicit reservoir-operation models that treat human management as signal rather than noise?

## Related

- [[overview]]
- [[topics/china-hydrology-datasets]]
- [[topics/precipitation-forcing-error-propagation]]
- [[topics/river-flow-connectivity]]
- [[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]]
- [[sources/2022-model-estimates-of-chinas-terrestrial-water-storage-variation-due-to-reservoir-operation]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]
