---
title: "Model estimates of China's terrestrial water storage variation due to reservoir operation"
type: source
status: active
created: 2026-04-09
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2022-model-estimates-of-chinas-terrestrial-water-storage-variation-due-to-reservoir-operation.pdf"
---

# Model estimates of China's terrestrial water storage variation due to reservoir operation

## Summary

This paper shifts the focus from natural runoff or streamflow reconstruction toward human-managed water storage. It develops a continental-scale land surface-hydrologic model for mainland China that explicitly represents `3,547` reservoirs with a calibration-free operation scheme for ungauged reservoirs, then uses a 30-year simulation to estimate how reservoir water storage contributes to China's terrestrial water storage variation.

## Key Claims

- The study presents a mainland-China-scale model that explicitly couples `3,547` reservoirs, covering over `90%` of China's combined reservoir capacity as of 2011.
- A calibration-free conceptual reservoir operation scheme can be used to simulate ungauged reservoirs at continental scale without requiring historical operation records for each reservoir.
- The coupled model is reported to reproduce streamflow, reservoir storage, and GRACE-based terrestrial water storage anomalies with satisfactory accuracy.
- China's seasonal reservoir water storage variation is estimated as roughly `15%`, `16%`, and `25%` of terrestrial water storage variation during `1981-1990`, `1991-2000`, and `2001-2010`, respectively.
- About one-fifth of China's reservoir capacity is estimated to be effectively used during a typical year, and reservoirs are argued to play a growing role in modulating the national water cycle over time.
- Despite that aggregate growth, the paper estimates that about `80 million` people live in regions where reservoir regulation of the seasonal water cycle weakened over recent decades.

## Methods And Evidence

- Uses the `CLHMS` land surface-hydrologic model over mainland China at `10 km` spatial resolution for a `1981-2010` simulation period.
- Represents reservoirs with a two-way coupled scheme so reservoir storage and releases interact with the broader terrestrial water cycle rather than being treated only as an outlet-flow correction.
- Activates each reservoir in the simulation according to its real-world completion year rather than assuming a static reservoir network.
- Proposes a calibration-free conceptual operation scheme for ungauged reservoirs and validates it against observed storage for `18` reservoirs whose combined capacity exceeds `30%` of China's total reservoir capacity as of 2011.
- Evaluates the coupled workflow against gauged streamflow, reservoir storage observations, and GRACE-derived terrestrial water storage anomalies at annual and seasonal scales.
- Frames the main question around the role of reservoir water storage in seasonal terrestrial water storage variation across time periods and spatial scales, not only around streamflow regulation.

## Why It Matters

- This paper adds a human-water-management layer that is largely absent from the other seeded sources in this wiki, which mostly emphasize natural runoff, natural streamflow, forcing error, or downstream connectivity.
- It is useful for this vault because it makes reservoir operation itself a first-class modeled storage process rather than treating human influence only as something to remove through naturalization.
- It also provides a bridge between hydrological reconstruction questions and broader terrestrial-water-storage or water-security questions, especially where reservoir operation materially reshapes seasonal storage dynamics.

## Tensions Or Caveats

- This is not a natural-flow dataset paper, so it should not be conflated with the wiki's reconstruction-oriented sources even though it uses a large-scale hydrologic modeling framework.
- The calibration-free reservoir-operation scheme is a major practical contribution, but it still abstracts highly heterogeneous real-world operating rules into a conceptual form.
- Validation against `18` reservoirs is meaningful at national scale because they represent a large share of capacity, but it still leaves uncertainty about smaller reservoirs and local operating behaviors.
- The paper focuses on seasonal terrestrial water storage variation over `1981-2010`, so its findings should not be read as direct validation of annual trends, newer decades, or specific basin-scale policy claims without care.

## Open Questions

- How should this wiki compare naturalization-oriented products with explicitly human-managed storage models without blurring their different aims?
- Which parts of China's terrestrial water storage variation remain weakly explained even after reservoir operation is modeled explicitly?
- How compatible is this reservoir-operation framework with the later natural-streamflow and connectivity workflows already in the wiki?
- When later papers discuss human impacts on flow or storage, are they extending this modeling line, the natural-flow reconstruction line, or a distinct branch altogether?

## Related

- [[overview]]
- [[topics/china-hydrology-datasets]]
- [[topics/natural-streamflow-reconstruction]]
- [[sources/2021-cnrd-v1-0-a-high-quality-natural-runoff-dataset-for-hydrological-and-climate-studies-in-china]]
- [[sources/2022-high-quality-reconstruction-of-chinas-natural-streamflow]]
- [[sources/2025-warming-climate-and-water-withdrawals-threaten-river-flow-connectivity-in-china]]
