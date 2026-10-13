---
layout: page
title: Robust Subspace Recovery
description: Implicit regularization and recovery of unknown-dimensional subspaces from outliers.
img: assets/img/Prop.jpg
importance: 8
category: research
---

High-dimensional observations often lie near a low-dimensional subspace, but outliers can make that structure difficult to recover. I study algorithms that recover the underlying representation while also identifying its dimension.

## Recovering a subspace of unknown dimension

Our ICLR 2022 work studies Dual Principal Component Pursuit (DPCP), which estimates directions orthogonal to the underlying subspace. By relaxing orthogonality constraints and using random initialization, multiple projected subgradient iterations can recover a sufficiently diverse collection of these directions.

Under the paper's assumptions, this collection spans the subspace's orthogonal complement with high probability. The algorithm therefore reveals the unknown codimension through its implicit regularization, connecting robust representation learning with optimization geometry.

<div class="row">
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/orth_DPCP.jpg" alt="Subspace recovered by orthogonal DPCP" class="img-fluid rounded z-depth-1" %}
  </div>
  <div class="col-sm mt-3 mt-md-0">
    {% include figure.html path="assets/img/Prop.jpg" alt="Subspace recovered by the proposed projected subgradient approach" class="img-fluid rounded z-depth-1" %}
  </div>
</div>
<div class="caption">
  Orthogonal DPCP (left) and the proposed approach for unknown codimension (right).
</div>

## Selected publication

- Paris Giampouras, Benjamin Haeffele, and René Vidal. [**Implicit Bias of Projected Subgradient Method Gives Provable Robust Recovery of Subspaces of Unknown Codimension**](https://openreview.net/forum?id=vA7doMdgi75). ICLR 2022, spotlight.
