---
layout: page
title: Tensors
description: Continual Learning: Theory and Algorithms
img: assets/img/CL_paper_graphic.001.png
redirect: 
importance: 4
category: research
---

This project aims a) to provide  theoretical insights into current state of the art continual learning algorithms and b) build on these insights to come up with novel and efficient  continual learning algorithms.



1. Theory of Continual Learning

The goal of continual learning is to find a model that solves multiple learning tasks which are presented sequentially to the learner. A key challenge in this setting is that the learner may \textit{forget} how to solve a previous task when learning a new task, a phenomenon known as \textit{catastrophic forgetting}. To address this challenge, many practical  methods have been proposed, including memory-based, regularization-based, and expansion-based methods. However, a rigorous theoretical understanding of these methods remains elusive. This paper aims to bridge this gap between theory and practice by proposing a new continual learning framework called \textit{Ideal Continual Learner (ICL)}, which is guaranteed to avoid catastrophic forgetting by construction. We show that ICL unifies multiple well-established continual learning methods and gives new theoretical insights into the strengths and weaknesses of these methods. We also derive generalization bounds for $\ICL$ which allow us to theoretically quantify \textit{how rehearsal affects generalization}. Finally, we connect ICL to several classic subjects and research topics of modern interest, which allows us to make historical remarks and inspire future directions.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/connection.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
<div class="caption">
    the Block-Term tensor Decomposition model (BTD) 
</div>
    
    
    
2. A Clustering-based Task Agnostic Continual Learning Algorithm    
    
We consider the problem of learning multiple tasks in a continual learning setting in which data from different tasks is presented to the learner in a streaming fashion. A key challenge in this setting is the so-called ``catastrophic forgetting problem", in which the performance of the learner in an ``old task" decreases when subsequently trained on a ``new task". In this paper, we alleviate the need to provide the algorithm with information about task changes while requiring constant memory about prior tasks by dynamically updating a finite pool of samples or gradients in a task-agnostic manner using a simple and efficient online clustering-based approach.     
    
    <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/CL_paper_graphic.001.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
   </div>
    <div class="caption">
        A Clustering-based Task Agnostic Continual Learning Algorithm 
    </div>


    
[1] L. Peng, P. V. Giampouras, R. Vidal, ``The Ideal Continual Learner: An Agent that Never Forgets", ICML, 2023<br />
 
[2] C. Laamers, R. Vidal, N. Belbachir, N. van Stein, T. Baeck, P. V. Giampouras, ``A Clustering-based Task Agnostic Continual Learning Algorithm, (under review), 2023<br/>




