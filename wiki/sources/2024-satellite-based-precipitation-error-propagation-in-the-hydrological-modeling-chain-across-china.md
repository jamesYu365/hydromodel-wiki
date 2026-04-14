---
title: "Satellite-based precipitation error propagation in the hydrological modeling chain across China"
type: source
status: active
created: 2026-04-05
updated: 2026-04-10
sources:
  - "raw/papers/ingested/2024-satellite-based-precipitation-error-propagation-in-the-hydrological-modeling-chain-across-china.pdf"
---

# Satellite-based precipitation error propagation in the hydrological modeling chain across China

## Summary

This paper studies how satellite-precipitation errors propagate through the hydrological modeling chain in China, from precipitation to runoff and then to streamflow. Using ten satellite precipitation products and 366 catchments over 2001 to 2018, it shows that routing often dampens precipitation-error effects on streamflow relative to runoff, but that small, dry, water-limited catchments can still amplify forcing errors.

## Key Claims

- Satellite-based precipitation products can support hydrological modeling, but their uncertainty propagates differently across products and hydroclimate regimes.
- For most satellite products, precipitation error becomes smaller after routing when moving from runoff simulation to streamflow simulation.
- The paper reports a concrete example in which `αRMAE` decreases by about `26%`, from `0.58` to `0.43`, when routing is considered for the `PERSIANN-CDR` product.
- Across 366 Chinese catchments, the linear slope between precipitation error and simulated streamflow error is much smaller than the corresponding slope for runoff error.
- Drier, water-limited, and smaller catchments are more prone to amplification of satellite-forcing errors in streamflow simulation.

## Methods And Evidence

- Evaluates ten satellite precipitation products, including both gauge-adjusted and non-gauge-adjusted products.
- Uses a combined land-surface and routing-model framework to track error propagation through precipitation, runoff, basin-averaged precipitation, and streamflow.
- Frames the work around three questions: differences among products, differences between runoff-stage and streamflow-stage propagation, and the factors that control propagation magnitude.
- Uses 366 catchments across China, which broadens national-scale evidence beyond a small set of basins.

## Why It Matters

- This paper helps interpret the reliability of hydrological datasets in this wiki by showing that forcing uncertainty does not transfer mechanically into hydrological output.
- It is especially relevant for any later comparison between runoff and streamflow products, because routing can dampen or reshape forcing error rather than simply passing it through.
- It gives a more realistic view of where satellite precipitation is risky: not uniformly everywhere, but especially in dry and water-limited settings.

## Tensions Or Caveats

- Better streamflow behavior after routing does not mean the forcing itself is accurate; it may mean the hydrological chain dampens some of the error.
- The paper studies propagation behavior from 2001 to 2018, so its conclusions do not directly validate older-period reconstructions such as 1961 to 2018 products without care.
- Different satellite products mix gauge-adjusted and non-adjusted designs, so product comparisons include both sensing differences and correction-strategy differences.

## Open Questions

- How should forcing-error propagation results change our trust in runoff versus streamflow datasets elsewhere in the wiki?
- Which of the ten precipitation products align best with the datasets already entering this vault?
- How should dry-region amplification affect interpretation of China-wide hydroclimate conclusions?

## Related

- [[overview]]
- [[topics/precipitation-forcing-error-propagation]]
- [[topics/china-hydrology-datasets]]
- [[topics/natural-streamflow-reconstruction]]
