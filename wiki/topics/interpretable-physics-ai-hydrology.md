---
title: "Interpretable Physics-AI Hydrology"
type: topic
status: active
created: 2026-04-14
updated: 2026-04-14
sources:
  - "[[sources/2024-a-mass-conserving-perceptron-for-machine-learning-based-modeling-of-geoscientific-systems]]"
  - "[[sources/2026-distilling-hydrological-and-land-surface-model-parameters-from-physio-geographical-properties-using-text-generating-ai]]"
---

# Interpretable Physics-AI Hydrology

## Summary

This topic tracks approaches that try to combine the flexibility of machine learning with the structural legibility of physical-conceptual hydrology. In this wiki, the key question is not simply whether AI can improve predictive skill, but whether it can do so while preserving explicit scientific hypotheses about conservation laws, architecture, parameterization, and process meaning.

## Key Points

- A central tension in modern hydrology is the tradeoff between predictive performance and scientific interpretability.
- One strategy is to design ML architectures whose internal structure already reflects hydrological constraints such as conservation and directed state-flux organization.
- Another strategy is to keep the process-based model structure but use AI to learn specific functions or transfer relationships that were previously hand-specified.
- The `MCP` paper represents the first strategy: interpretable learnable building blocks for mass-conserving recurrent models.
- The 2026 Feigl et al. paper represents the second strategy: AI-assisted discovery of interpretable transfer functions inside a process-based regionalization workflow.
- These approaches are related but not identical: one is about model architecture, the other about process or parameter function specification.

## Evidence Base

- [[sources/2024-a-mass-conserving-perceptron-for-machine-learning-based-modeling-of-geoscientific-systems]] proposes the `MCP` as a physically interpretable recurrent unit that embeds mass conservation into ML-based geoscientific modeling and uses it for parsimonious rainfall-runoff representation plus hypothesis testing.
- [[sources/2026-distilling-hydrological-and-land-surface-model-parameters-from-physio-geographical-properties-using-text-generating-ai]] shows that generative AI can be used to discover explicit transfer functions for a process-based hydrological model while retaining readable equations and benchmarking against a regional `LSTM`.

## Open Questions

- Which parts of hydrological model development benefit most from AI: architecture design, function specification, parameter regionalization, or direct prediction?
- How much conservation or process structure should be hard-coded before model flexibility becomes too constrained?
- When should interpretable physics-AI approaches be preferred over high-performing but less legible `LSTM`-style models?
- What evaluation setup best tests whether an interpretable AI-hydrology method actually improves scientific understanding rather than only accuracy?

## Related

- [[overview]]
- [[topics/hydrological-parameter-regionalization]]
- [[sources/2024-a-mass-conserving-perceptron-for-machine-learning-based-modeling-of-geoscientific-systems]]
- [[sources/2026-distilling-hydrological-and-land-surface-model-parameters-from-physio-geographical-properties-using-text-generating-ai]]
