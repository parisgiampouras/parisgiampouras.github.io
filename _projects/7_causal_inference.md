---
layout: page
title: Causal Inference & Transportability
description: Robust causal abstractions and transferring causal conclusions across populations.
img: assets/img/project-causal-inference.png
importance: 3
category: research
---

Causal models express how a system responds to interventions. My research develops abstractions that relate these models across levels of detail and studies when causal conclusions remain useful across changing environments and populations.

## Distributionally robust causal abstractions

Our **ICML 2026** work develops causal abstraction methods that account for environmental shifts and model misspecification. We formulate learning as a constrained min-max problem with Wasserstein ambiguity sets and derive guarantees on worst-case abstraction error.

This provides a way to reason about the reliability of an abstraction when the assumed environment or model is imperfect.

## Generalised transportability

Our transportability work takes a model-level perspective: can one abstraction map align the interventional behaviour of a source and target population?

When exact alignment is unavailable, we derive certified intervals for causal queries. The framework also addresses settings where a query is not exactly transportable or target data are unavailable, under explicit assumptions on mechanism and environment perturbations.

## Selected publications

- Yorgos Felekis, Theodoros Damoulas, and Paris Giampouras. [**Distributionally Robust Causal Abstractions**](https://proceedings.mlr.press/v306/felekis26a.html). ICML 2026.
- Yorgos Felekis, Paris Giampouras, Fabio Massimo Zennaro, and Theodoros Damoulas. [**Generalised Transportability via Causal Abstractions**](https://arxiv.org/abs/2608.15645). arXiv, 2026.
