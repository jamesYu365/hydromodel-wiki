---
title: "China Hydrology Datasets"
type: topic
status: active
created: 2026-04-05
updated: 2026-04-05
sources:
  - "[[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]]"
  - "[[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]"
  - "[[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]"
  - "[[sources/2024-satellite-based-precipitation-error-propagation-in-the-hydrological-modeling-chain-across-china]]"
  - "[[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]]"
  - "[[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]"
---

# China Hydrology Datasets

## Summary

This topic tracks datasets used to describe Chinese runoff and streamflow, especially products intended for climate analysis, hydrological modeling, and water-resources assessment. A recurring theme is the tension between broad coverage and the quality of natural-flow representation.

## Key Points

- Existing global runoff and streamflow products often have uneven station coverage and data gaps in China.
- China-focused datasets can provide stronger local calibration and better treatment of human disturbance, but they differ in scope, resolution, and reconstruction assumptions.
- `CNRD v1.0` provides gridded natural runoff at `0.25°` resolution and daily/monthly/annual scales for 1961 to 2018, giving this wiki a public runoff-oriented reference product.
- The 2022 Miao et al. dataset is a foundational entry in this wiki because it provides long-term reconstructed monthly natural streamflow across 330 catchments.
- Its supplementary materials are also important because they expose the data-quality logic, station composition, and post-processing details behind the dataset.
- The 2024 precipitation-error paper adds a forcing-quality perspective, showing that precipitation uncertainty propagates differently into runoff and streamflow outputs across China.
- The 2025 connectivity paper uses this modeling lineage as an application layer, turning reconstructed flow into claims about intermittency, connectivity, and withdrawal pressure across a national river network.
- Its supporting information shows that the application layer also involved a materially expanded modeling workflow rather than just reusing the 2022 setup unchanged.

## Evidence Base

- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]] positions its contribution against global products such as GRDB, GSIM, and other runoff reconstructions that are weaker for China-specific natural-flow analysis.
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]] adds the operational detail needed to compare this dataset fairly with later China-specific products.
- [[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]] adds a public gridded runoff product that should be compared with the 2022 streamflow reconstruction rather than conflated with it.
- [[sources/2024-satellite-based-precipitation-error-propagation-in-the-hydrological-modeling-chain-across-china]] adds the missing forcing-error layer needed to interpret why some hydrological products may look more or less reliable downstream.
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]] shows how these datasets and models can be used to answer higher-level ecological and water-management questions.
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]] adds the methodological detail needed to judge whether 2025 should be viewed as a simple update, a workflow extension, or both.

## Open Questions

- How should later datasets in this wiki be compared: by spatial coverage, temporal resolution, naturalization quality, or intended application?
- What comparison frame is most useful here: gridded runoff versus routed streamflow, or public dataset usability versus reconstruction fidelity?
- Which later papers extend, refine, or challenge the 2022 reconstruction scheme?
- Which dataset differences are methodological versus merely documentation differences?
- How much of observed dataset quality is really about forcing quality versus routing, calibration, or post-processing?
- When should an application paper be represented as a dataset/method update versus as a downstream use case built on earlier products?
- How should the wiki represent workflow evolution when a later paper both reuses and materially extends earlier reconstruction methods?

## Related

- [[overview]]
- [[topics/natural-streamflow-reconstruction]]
- [[topics/precipitation-forcing-error-propagation]]
- [[topics/river-flow-connectivity]]
- [[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow-supplementary-materials]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]
