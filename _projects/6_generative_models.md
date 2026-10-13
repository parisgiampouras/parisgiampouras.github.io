---
layout: page
title: Generative Models & Alignment
description: Semantic guidance, inverse problems, and efficient adaptation of diffusion and flow models.
img: assets/img/project-generative-alignment.png
importance: 1
category: research
---

I study how pretrained generative models can be aligned and adapted to solve problems with limited observations or additional constraints. My work connects representation learning and optimization with diffusion and flow-based models.

## Align & Invert

[**Align & Invert**](https://arxiv.org/abs/2511.16870), accepted to **NeurIPS 2026**, brings representation alignment to inference-time inverse problems. We use semantic features from a pretrained DINOv2 encoder to guide reconstruction with diffusion and flow models.

Because the clean image is unavailable, the method constructs approximate semantic targets and aligns them with model representations during reconstruction. We evaluate the approach on super-resolution, inpainting, and deblurring, improving reconstruction quality and perceptual realism across several solvers.

The analysis connects alignment with distribution matching in semantic feature space and explains how alignment updates steer latent states toward clean-image states under regularity assumptions.

## Post-training and efficient adaptation

Current directions include post-training and parameter-efficient adaptation of diffusion and flow models using low-rank and tensor parameterizations. I am interested in how these approaches support controllable generation and adaptation to new tasks and domains.

I also co-organized the [ReALM–GEN workshop at ICLR 2026](https://realm-gen-workshop.github.io/), focused on constrained and preference-aligned generative models.

## Selected publication

- Loukas Sfountouris, Giannis Daras, and Paris Giampouras. [**Align & Invert: Solving Inverse Problems with Diffusion and Flow-based Models via Representation Alignment**](https://arxiv.org/abs/2511.16870). NeurIPS 2026.
