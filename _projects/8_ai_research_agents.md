---
layout: page
title: AI Research Agents
description: Reasoning, experiment selection, and efficient automated machine-learning research.
img: assets/img/project-ai-research-agents.png
importance: 2
category: research
---

At Meta FAIR, I work on AI research agents that propose, implement, and evaluate machine-learning experiments. A central question is how an agent should allocate limited computation when it can generate more candidate solutions than it can afford to test.

## AI Research Preference Models

Our work on **AI Research Preference Models** compares candidate research solutions before committing to expensive evaluations. We study two approaches: an inference-only model that reasons over plans, code, and previous results, and an agentic variant that also runs small pilot experiments.

Integrated into the AIRA-dojo agent, these models improve research performance on AIRS-Bench. In the reported experiments, they reach the unguided agent's 24-hour performance in roughly 15 hours, using less than two-thirds of its execution budget.

## Adaptive research systems

My broader interests include test-time reasoning, learning from feedback, and continual adaptation. I aim to connect these ideas with agents that improve their research decisions through iterative experimentation and evaluation.

## Selected publication

- Thomas Simon Foster et al. [**AI Research Preference Models**](https://arxiv.org/abs/2608.13940). arXiv, 2026.
