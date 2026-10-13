---
layout: page
title: Low-Rank Learning & Optimization
description: Matrix factorization, implicit regularization, and efficient optimization with guarantees.
img: assets/img/graphic_neurips.jpg
importance: 4
category: research
---

Low-rank structure represents high-dimensional data and parameters using compact factors. I develop optimization methods that exploit this structure, identify model complexity, and remain reliable under corrupted measurements.

## Robust recovery with unknown rank

Our ICML 2025 work analyzes an overparameterized, preconditioned subgradient algorithm for recovering asymmetric low-rank matrices from corrupted measurements. The analysis establishes linear convergence rates independent of the true rank under the stated assumptions, addressing recovery when the rank is unknown.

## Nonconvex low-rank regularization

Our NeurIPS 2020 work develops a variational representation of the Schatten-$p$ quasi-norm for $p \in (0,1]$. Expressing the regularizer through matrix factors connects rank selection to group sparsity and enables algorithms that avoid repeated singular value decompositions.

{% include figure.html path="assets/img/graphic_neurips.jpg" alt="Variational low-rank matrix factorization framework" class="img-fluid rounded z-depth-1" %}

## Parameter-efficient adaptation

A current research direction is to use low-rank structure for parameter-efficient fine-tuning of foundation models, including language, diffusion, and flow-based models. This connects my work on structured optimization with efficient model adaptation.

## Selected publications

- Paris Giampouras, Hanqin Cai, and René Vidal. [**Guarantees of a Preconditioned Subgradient Algorithm for Overparameterized Asymmetric Low-rank Matrix Recovery**](https://proceedings.mlr.press/v267/giampouras25a.html). ICML 2025.
- Paris Giampouras, René Vidal, Athanasios Rontogiannis, and Benjamin Haeffele. [**A Novel Variational Form of the Schatten-p Quasi-Norm**](https://proceedings.neurips.cc/paper/2020/file/f53eb4122d5e2ce81a12093f8f9ce922-Paper.pdf). NeurIPS 2020.
- Paris Giampouras, Athanasios Rontogiannis, and Konstantinos Koutroumbas. [**Alternating Iteratively Reweighted Least Squares Minimization for Low-Rank Matrix Factorization**](https://doi.org/10.1109/TSP.2018.2883921). IEEE Transactions on Signal Processing, 2019.
