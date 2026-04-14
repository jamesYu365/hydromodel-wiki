---
title: "A mass-conserving-perceptron for machine-learning-based modeling of geoscientific systems"
type: source
status: active
created: 2026-04-14
updated: 2026-04-14
sources:
  - "raw/papers/ingested/2024-a-mass-conserving-perceptron-for-machine-learning-based-modeling-of-geoscientific-systems.pdf"
---

# A mass-conserving-perceptron for machine-learning-based modeling of geoscientific systems

## Summary

This paper proposes the `Mass-Conserving-Perceptron` (`MCP`) as an interpretable computational unit for machine-learning-based geoscientific modeling. The core idea is to bridge physical-conceptual rainfall-runoff modeling and gated recurrent neural networks by using a node architecture that explicitly respects mass conservation while still allowing the functional forms of system processes to be learned from data.

## Key Claims

- A physically interpretable `MCP` unit can serve as a basic building block for ML-based modeling of mass-conserving geoscientific systems.
- The `MCP` exploits the directed-graph similarity between physical-conceptual models and gated recurrent neural networks to combine explicit conservation structure with learned process functions.
- Even a single-`MCP`-node model can parsimoniously represent rainfall-runoff dynamics in the `Leaf River Basin` while maintaining interpretability.
- The framework supports scientific hypothesis testing by allowing model structure to be varied systematically and examined as a sequence of explicit representational choices.
- The concept is presented as extensible beyond mass flows toward coupled mass-energy-information representations in geoscientific systems.

## Methods And Evidence

- Frames both physical-conceptual hydrological models and recurrent neural networks as directed graphs of nodes and links, then designs the `MCP` as a node type suited to mass-conserving systems.
- Builds the `MCP` to include recurrence, nodal conservation constraints, learnable unobserved losses, LSTM-like gating, and learnable flux-equation behavior.
- Tests the concept as a proof of concept on catchment-scale rainfall-runoff modeling for the `Leaf River Basin` in Mississippi.
- Emphasizes not just predictive skill but also functional expressivity, parsimony, and the ability to interpret internal system behavior.
- Positions the approach against both traditional physical-conceptual hydrology and more opaque ML approaches such as `LSTM` or `GRNN` models.
- Argues that model development should move beyond pure parameter optimization toward `function space optimization`, where the structural form of process relationships becomes learnable.

## Why It Matters

- This paper is useful in this wiki because it offers a concrete architecture for making ML-based hydrological models more physically legible rather than only more accurate.
- It complements the later 2026 transfer-function paper by addressing a different layer of the modeling problem: not just how to regionalize parameters, but how to design model building blocks whose internal behavior remains scientifically inspectable.
- It also sharpens an important distinction in this vault between using AI as a black-box predictor and using AI as a structured component inside a physically interpretable modeling framework.

## Tensions Or Caveats

- The proof of concept is intentionally narrow, centered on the `Leaf River Basin`, so the paper is more a framework proposal than a broad large-sample validation study.
- The paper argues for interpretability, but that claim depends on accepting the chosen graph structure and conservation assumptions as meaningful approximations of the target system.
- Single-node parsimony is appealing, but the paper itself notes that careful training and further work are needed before treating the approach as mature for wide deployment.
- Although the framework is pitched as extensible to coupled mass-energy-information flows, the present paper mainly demonstrates mass conservation and rainfall-runoff behavior.

## Open Questions

- How well do `MCP`-based directed-graph models scale from single-basin proof of concept to large-sample hydrology?
- When does enforcing conservation structure improve extrapolation, and when does it mainly reduce functional flexibility?
- How should `MCP`-style architectures be compared with differentiable hydrology, mass-conserving `LSTM` variants, or explicit symbolic-regression approaches?
- What is the minimal graph complexity needed for different hydroclimatic regimes if the goal is interpretable rather than merely accurate hydrological learning?

## Related

- [[overview]]
- [[topics/interpretable-physics-ai-hydrology]]
- [[topics/hydrological-parameter-regionalization]]
- [[sources/2026-distilling-hydrological-and-land-surface-model-parameters-from-physio-geographical-properties-using-text-generating-ai]]
