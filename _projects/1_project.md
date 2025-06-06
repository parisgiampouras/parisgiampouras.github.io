---
layout: page
title: Robust Subspace Recovery
description: Recovering Subspaces of Unknown Dimension in The Presence of Outliers
img: assets/img/Prop.jpg
importance: 1
category: research
---

Robust subspace recovery (RSR) is a fundamental problem in robust representation learning. Here we focus on a recently proposed RSR method termed Dual Principal Component Pursuit (DPCP) approach, which aims to recover a basis of the orthogonal complement of the subspace and is amenable to handling subspaces of high relative dimension. Prior work has shown that DPCP can provably recover the correct subspace in the presence of outliers, as long as the true dimension of the subspace is known. We show that DPCP can provably solve RSR problems in the unknown subspace dimension regime, as long as orthogonality constraints adopted in previous DPCP formulations- are relaxed and random initialization is used instead of spectral one. Namely, we propose a very simple algorithm based on running multiple instances of a projected sub-gradient descent method (PSGM), with each problem instance seeking to find one vector in the null space of the subspace. We theoretically prove that under mild conditions this approach will succeed with high probability. In particular, we show that 1) all of the problem instances will converge to a vector in the nullspace of the subspace and 2) the ensemble of problem instance solutions will be sufficiently diverse to fully span the nullspace of the subspace thus also revealing its true unknown codimension.We provide empirical results that corroborate our theoretical results and showcase the remarkable implicit rank regularization behavior of PSGM algorithm that allows us to perform RSR without being aware of the subspace dimension.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/orth_DPCP.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
   
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Prop.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    
</div>
 <div class="caption">
   (left) Orhogonal DPCP [1] and (right) Proposed DPCP [2]
</div>

[1] Zhihui Zhu, Tianyu Ding, Daniel Robinson, Manolis Tsakiris, René Vidal, "A Linearly Convergent Method for Non-Smooth Non-Convex Optimization
on the Grassmannian with Applications to Robust Subspace and Dictionary Learning", NeurIPS, 2019.
[2] Paris Giampouras, Benjamin Haeffele, Rene Vidal, "Implicit Bias of Projected Subgradient Method Gives Provable Robust Recovery of Subspaces of Unknown Codimension", ICLR, 2022. 
