---
layout: page
title: Tensor Decomposition
description: Structured representations, automatic rank selection, and online learning.
img: assets/img/Bayesian_BTD.jpg
importance: 5
category: research
---

Tensor decompositions provide structured representations of multiway data and model parameters. My work focuses on estimating both the factors and the model complexity, including the number of components and their ranks.

## Learning the structure of block-term models

Block-term decompositions represent data using components whose multilinear ranks can differ. We develop methods that promote sparsity jointly across factor columns, allowing the model structure to emerge during optimization.

Our work includes a block successive upper-bound minimization approach and a Bayesian formulation based on hierarchical sparsity and variational inference. The Bayesian method jointly estimates the decomposition and its ranks while avoiding manual regularization-parameter tuning.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/BTD.jpg" alt="Block-term tensor decomposition" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">The block-term tensor decomposition model.</div>

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/Bayesian_BTD.jpg" alt="Hierarchical Bayesian model for tensor rank selection" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">Hierarchical Bayesian modelling for automatic structure and rank estimation.</div>

## Online learning and model adaptation

We also develop online rank-revealing methods for streaming data, allowing the decomposition to adapt as observations arrive. A current interest is to extend structured tensor parameterizations to parameter-efficient adaptation of foundation models.

## Selected publications

- Athanasios Rontogiannis, Eleftherios Kofidis, and Paris Giampouras. [**Block-Term Tensor Decomposition: Model Selection and Computation**](https://doi.org/10.1109/JSTSP.2021.3051488). IEEE Journal of Selected Topics in Signal Processing, 2021.
- Paris Giampouras, Athanasios Rontogiannis, and Eleftherios Kofidis. [**Block-Term Tensor Decomposition Model Selection and Computation: The Bayesian Way**](https://doi.org/10.1109/TSP.2022.3159029). IEEE Transactions on Signal Processing, 2022.
- Athanasios Rontogiannis, Eleftherios Kofidis, and Paris Giampouras. **Online Rank-Revealing Block-Term Tensor Decomposition**. Signal Processing, 2023.




