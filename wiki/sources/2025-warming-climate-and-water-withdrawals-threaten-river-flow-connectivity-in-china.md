---
title: "Warming climate and water withdrawals threaten river flow connectivity in China"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china.pdf"
  - "[[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]"
---

# Warming climate and water withdrawals threaten river flow connectivity in China

## Summary

This paper applies reconstructed natural streamflow and related hydrological modeling to a larger ecological and water-management question: how climate warming and human water withdrawals change river flow connectivity across China. It analyzes 217,001 river reaches from 1961 to 2020 and argues that warming and withdrawals materially increase intermittency risk, even when long-term precipitation trends would otherwise lengthen connectivity.

## Key Claims

- About `13%` of river reaches in mainland China are naturally intermittent, with strong north-south contrast.
- River intermittency decreased slightly over 1961 to 2020 under the raw simulation, but warming offset part of that improvement by reducing surface-water persistence.
- Removing the long-term temperature trend roughly doubles the decline in intermittent-river length, from about `-233 km/y` in the raw simulation to about `-476 km/y`, implying that warming counteracted the connectivity gains that would otherwise have occurred.
- When agricultural, domestic, and industrial withdrawals plus environmental-flow requirements are considered, the length of intermittent rivers increases dramatically from `13%` to `50%`.
- Unregulated withdrawals are therefore presented as a major threat to river functional connectivity, especially in drying regions.

## Methods And Evidence

- Uses reconstructed natural streamflow to examine river-flow connectivity across `217,001` river reaches in China from `1961` to `2020`.
- Evaluates both natural intermittency patterns and the effects of warming trends and sectoral water withdrawals.
- Uses a revised dendritic connectivity index (`DCI`) and zero-flow conditions to characterize spatial and temporal river-network connectivity.
- Extends the earlier reconstruction line from catchment-scale streamflow estimation toward river-network-scale ecological and functional interpretation.
- The supporting information shows that this workflow reuses the naturalization lineage but extends calibration/validation to `651` stations and adds an upstream-downstream scaled bias-correction (`UDSBC`) procedure.
- The supporting information also shows that low-flow-focused metrics (`LogCC`, `LogNSE`, `Pbias`, `LogKGE`) were chosen explicitly to better represent intermittence.

## Why It Matters

- This paper shows how the earlier reconstruction/modeling work in this wiki becomes useful for a higher-level national inference rather than only for hydrological dataset construction.
- It reframes natural-flow datasets as infrastructure for ecological and water-governance analysis, not just hydrological benchmarking.
- It also makes clear that climate and human withdrawal pressures should be interpreted jointly rather than as isolated drivers.

## Tensions Or Caveats

- This is an application-layer result, so its reliability partly inherits the assumptions and weaknesses of the upstream reconstructed streamflow/modeling framework.
- The paper uses modeled connectivity over a huge river network, which increases scope but also increases dependence on the validity of routing, forcing, and withdrawal assumptions.
- The connectivity findings are not just “an update” of the 2022 product; they are a downstream analysis built on related modeling ideas and should be linked accordingly rather than treated as the same artifact.
- The supplement makes clear that bias correction (`UDSBC`) is part of the workflow, so some downstream connectivity skill may depend on post-processing as well as on the raw model.

## Open Questions

- Exactly how much of the reported connectivity pattern depends on `UDSBC` and the low-flow metric choices?
- How sensitive are the connectivity conclusions to assumptions about water-withdrawal estimates and environmental-flow requirements?
- How should this paper be compared fairly with the earlier 2022 reconstruction workflow, given the larger 651-station basis and added post-processing?

## Related

- [[overview]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china-supporting-information]]
- [[topics/river-flow-connectivity]]
- [[topics/natural-streamflow-reconstruction]]
- [[topics/china-hydrology-datasets]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
