---
layout: page
title: Robust Probabilistic Inference
description: Generalised variational inference, federated learning, and uncertainty under misspecification.
img: assets/img/project-probabilistic-inference.png
importance: 7
category: research
---

Probabilistic learning should remain useful when its assumptions about the prior or likelihood are imperfect. My research studies generalised variational inference and federated learning, combining algorithm design with analysis of robustness and posterior concentration.

## Federated generalised variational inference

FedGVI provides a probabilistic federated-learning framework that accounts for prior and likelihood misspecification. It generalizes partitioned variational inference and studies how divergence choices can support robust updates across distributed clients.

The work combines theoretical analysis with experiments on synthetic and real classification datasets and was presented as an **ICML 2025 spotlight**.

## Posterior convergence under prior misspecification

We also study existence, uniqueness, and concentration of generalised variational inference posteriors. The analysis includes cases in which misspecified priors lead to inconsistent Bayesian posteriors, providing conditions under which generalised inference still concentrates near loss minimizers.

## Selected publications

- Terje Mildner, Oliver Hamelijnck, Paris Giampouras, and Theodoros Damoulas. [**Federated Generalised Variational Inference: A Robust Probabilistic Federated Learning Framework**](https://proceedings.mlr.press/v267/mildner25a.html). ICML 2025, spotlight.
- Terje Mildner, Paris Giampouras, and Theodoros Damoulas. [**Rates of Convergence of Generalised Variational Inference Posteriors under Prior Misspecification**](https://arxiv.org/abs/2510.03109). arXiv, 2025.
