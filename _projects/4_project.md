---
layout: page
title: Continual Learning & Adaptation
description: Sequential learning, retention of prior knowledge, and efficient model adaptation.
img: assets/img/CL_paper_graphic.001.png
importance: 6
category: research
---

AI systems encounter new tasks and changing environments throughout their lifetime. My research studies how they can adapt while retaining previously acquired knowledge, combining theoretical frameworks with practical learning algorithms.

## Foundations of continual learning

The Ideal Continual Learner framework formalizes learning without forgetting through an idealized construction. It unifies established approaches and clarifies the roles of memory, constraints, and model capacity. We also derive generalization bounds that quantify the effect of rehearsal.

<div class="row">
  <div class="col-sm-8 mx-auto mt-3">
    {% include figure.html path="assets/img/connection.png" alt="Connections between the Ideal Continual Learner and established methods" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## Adapting without explicit task boundaries

In domain-incremental learning, task changes may be unobserved. Our clustering-based approach maintains a finite pool of samples or gradients and uses online clustering to support task-agnostic versions of projection-based methods.

<div class="row">
  <div class="col-sm-10 mx-auto mt-3">
    {% include figure.html path="assets/img/CL_paper_graphic.001.png" alt="Clustering-based domain-incremental learning" class="img-fluid rounded z-depth-1" %}
  </div>
</div>

## Continual and parameter-efficient adaptation of LLMs

My current interests include continual adaptation of language models, structured parameter updates, and learning from feedback. These directions connect continual-learning foundations with post-training and the development of adaptive AI agents.

## Selected publications

- Liangzu Peng, Paris Giampouras, and René Vidal. [**The Ideal Continual Learner: An Agent That Never Forgets**](https://proceedings.mlr.press/v202/peng23a.html). ICML 2023.
- Christiaan Lamers, René Vidal, Nabil Belbachir, Niki van Stein, Thomas Bäeck, and Paris Giampouras. [**Clustering-Based Domain-Incremental Learning**](https://openaccess.thecvf.com/content/ICCV2023W/VCL/html/Lamers_Clustering-Based_Domain-Incremental_Learning_ICCVW_2023_paper.html). ICCV Workshop on Visual Continual Learning, 2023.
