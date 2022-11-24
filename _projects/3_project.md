---
layout: page
title: Tensor decomposition
description: Model Selection and Computation for Block-Term Tensor Decomposition
img: assets/img/BTD.jpg
redirect: 
importance: 3
category: research
---

The so-called block-term decomposition (BTD) tensor model has been recently receiving increasing attention due to its enhanced ability of representing systems and signals that are composed of blocks of rank higher than one, a scenario encountered in numerous and diverse applications. Its uniqueness and approximation have thus been thoroughly studied. Nevertheless, the challenging problem of estimating the BTD model structure, namely the number of block terms and their individual ranks, has only recently started to attract significant attention. In this papers, we propose novel methods for BTD model selection and computation. The main idea is leverage column sparsity jointly on the factors and in a hierarchical manner and estimating the ranks as the numbers of factor columns of non-negligible magnitude. The problem has been addressed via a block successive upper bound minimization (BSUM) approach and a fully automated Bayesian approach which alleviates the need for hyperparameter tuning.



<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/BTD.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/Bayesian_BTD.jpg" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
<div class="caption">
    (left) the Block-Term tensor Decomposition model (BTD) right) The hierarchical Bayesian network employed in [2]
</div>


[1] Athanasios A Rontogiannis, Eleftherios Kofidis, Paris V Giampouras, "Block-term tensor decomposition: Model selection and computation", IEEE Journal on Selected Topics on Signal Processing, 2021.
[2] Paris V Giampouras, Athanasios A Rontogiannis, Eleftherios Kofidis, "Block-Term Tensor Decomposition Model Selection and Computation: The Bayesian Way" IEEE Transactions on Signal Processing, 2022.




