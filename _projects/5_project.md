---
layout: page
title: Adversarial Robustness
description: Reverse engineering attacks through sparse recovery and generative-model inversion.
img: assets/img/project-adversarial-robustness.png
importance: 9
category: research
---

Reliable learning systems need methods for understanding and recovering from adversarial perturbations. My work studies how structured representations and generative priors can help separate a clean signal from an attack and identify the underlying threat model.

## Reverse engineering attacks with sparse models

Our ICML 2022 work formulates reverse engineering of adversarial attacks as a block-sparse recovery problem. Under geometric conditions on the signal and attack subspaces, the method can recover the clean signal and attack, classify the signal, and identify the attack type.

## Generative priors for nonlinear data

Our GAN inversion work extends this perspective to clean data modelled by a generative network. It combines latent inversion with block-sparse recovery and establishes deterministic linear convergence guarantees under the paper's conditions. This connects adversarial robustness with the optimization geometry of generative models.

## Selected publications

- Darshan Thaker, Paris Giampouras, and René Vidal. [**Reverse Engineering $\ell_p$ Attacks: A Block-Sparse Optimization Approach with Recovery Guarantees**](https://proceedings.mlr.press/v162/thaker22a.html). ICML 2022, equal contribution by Darshan Thaker and Paris Giampouras.
- Darshan Thaker, Paris Giampouras, and René Vidal. [**A Linearly Convergent GAN Inversion-based Algorithm for Reverse Engineering of Deceptions**](https://arxiv.org/abs/2306.04756). arXiv, 2023.






