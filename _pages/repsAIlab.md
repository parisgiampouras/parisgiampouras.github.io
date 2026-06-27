---
layout: page
title: RepsAI Lab
nav: true
description: Representational AI Lab
permalink: /repsai/
nav_order: 3
---

<style>
  /* ========= REPSAI PAGE ========= */

  .repsai-page {
    margin-top: 0.5rem;
  }

  .repsai-hero {
    display: grid;
    grid-template-columns: minmax(0, 1fr) 260px;
    gap: 2rem;
    align-items: center;
    margin: 1rem 0 2.6rem;
    padding: 2.4rem 2rem;
    border-radius: 1.5rem;
    background:
      radial-gradient(circle at top left, rgba(37, 99, 235, 0.14), transparent 34%),
      radial-gradient(circle at bottom right, rgba(14, 165, 233, 0.15), transparent 36%),
      linear-gradient(135deg, #f8fafc 0%, #eff6ff 100%);
    border: 1px solid rgba(148, 163, 184, 0.28);
    box-shadow: 0 14px 36px rgba(15, 23, 42, 0.08);
  }

  .repsai-kicker {
    display: inline-block;
    margin-bottom: 0.85rem;
    padding: 0.32rem 0.72rem;
    border-radius: 999px;
    font-size: 0.74rem;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: var(--global-theme-color, #2563eb);
    background: rgba(255, 255, 255, 0.78);
    border: 1px solid rgba(148, 163, 184, 0.28);
  }

  .repsai-hero h1 {
    margin: 0 0 1rem;
    font-size: clamp(1.85rem, 4vw, 3rem);
    line-height: 1.08;
    letter-spacing: -0.045em;
    font-weight: 800;
  }

  .repsai-subtitle {
    max-width: 760px;
    margin-bottom: 1.35rem;
    font-size: 1.03rem;
    line-height: 1.6;
    color: var(--global-text-color-light, #64748b);
  }

  .repsai-button {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    padding: 0.62rem 0.95rem;
    border-radius: 999px;
    font-size: 0.88rem;
    font-weight: 700;
    text-decoration: none !important;
    color: #fff !important;
    background: var(--global-theme-color, #2563eb);
    border: 1px solid var(--global-theme-color, #2563eb);
    box-shadow: 0 8px 20px rgba(15, 23, 42, 0.08);
  }

  .repsai-button:hover {
    transform: translateY(-1px);
    text-decoration: none !important;
  }

  .repsai-logo-wrap {
    text-align: center;
  }

  .repsai-logo {
    width: 230px;
    max-width: 230px;
    height: auto;
    border-radius: 1.25rem;
    box-shadow: 0 14px 30px rgba(15, 23, 42, 0.16);
    border: 4px solid rgba(255, 255, 255, 0.95);
  }

  .repsai-section {
    margin: 2.4rem 0 1.1rem;
  }

  .repsai-section h2 {
    margin-bottom: 0.65rem;
    font-weight: 800;
    letter-spacing: -0.02em;
  }

  .repsai-section p {
    font-size: 0.98rem;
    line-height: 1.65;
  }

  .repsai-card-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(215px, 1fr));
    gap: 1rem;
    margin: 1.2rem 0 2.4rem;
  }

  .repsai-topic-card {
    min-height: 190px;
    padding: 1.35rem 1.2rem;
    border-radius: 1.15rem;
    background: var(--global-card-bg-color, #ffffff);
    border: 1px solid var(--global-divider-color, rgba(148, 163, 184, 0.28));
    box-shadow: 0 8px 24px rgba(15, 23, 42, 0.055);
    transition: transform 0.16s ease, box-shadow 0.16s ease, border-color 0.16s ease;
  }

  .repsai-topic-card:hover {
    transform: translateY(-3px);
    border-color: rgba(37, 99, 235, 0.35);
    box-shadow: 0 14px 34px rgba(15, 23, 42, 0.085);
  }

  .repsai-icon {
    width: 2.3rem;
    height: 2.3rem;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 0.85rem;
    border-radius: 0.8rem;
    background: rgba(37, 99, 235, 0.10);
    font-size: 1.18rem;
  }

  .repsai-topic-card h3 {
    margin: 0 0 0.55rem;
    font-size: 1.05rem;
    font-weight: 750;
  }

  .repsai-topic-card p {
    margin: 0;
    font-size: 0.9rem;
    line-height: 1.55;
    color: var(--global-text-color-light, #64748b);
  }

  .member-subsection {
    margin-top: 1.9rem;
    margin-bottom: 0.8rem;
    font-size: 1.18rem;
    font-weight: 750;
  }

  .member-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(245px, 1fr));
    gap: 1rem;
    margin: 1rem 0 2rem;
  }

  .member-card {
    position: relative;
    min-height: 185px;
    padding: 1.25rem 1.15rem;
    border-radius: 1.15rem;
    background: var(--global-card-bg-color, #ffffff);
    border: 1px solid var(--global-divider-color, rgba(148, 163, 184, 0.28));
    box-shadow: 0 8px 24px rgba(15, 23, 42, 0.055);
    transition: transform 0.16s ease, box-shadow 0.16s ease, border-color 0.16s ease;
    overflow: hidden;
  }

  .member-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 14px 34px rgba(15, 23, 42, 0.085);
  }

  .member-card::before {
    content: "";
    position: absolute;
    top: 0;
    left: 0;
    width: 5px;
    height: 100%;
    background: #64748b;
  }

  .phd-card::before {
    background: #2563eb;
  }

  .intern-card::before {
    background: #ca8a04;
  }

  .external-card::before {
    background: #9333ea;
  }

  .msc-card::before {
    background: #16a34a;
  }

  .alumni-card::before {
    background: #64748b;
  }

  .member-label {
    display: inline-block;
    margin-bottom: 0.7rem;
    padding: 0.24rem 0.55rem;
    border-radius: 999px;
    font-size: 0.68rem;
    font-weight: 800;
    letter-spacing: 0.05em;
    text-transform: uppercase;
    color: var(--global-theme-color, #2563eb);
    background: rgba(37, 99, 235, 0.10);
  }

  .member-card h3 {
    margin: 0 0 0.45rem;
    font-size: 1.05rem;
    font-weight: 750;
    line-height: 1.25;
  }

  .member-card p {
    margin-bottom: 0.5rem;
    font-size: 0.9rem;
    line-height: 1.5;
  }

  .years {
    color: var(--global-text-color-light, #64748b);
    font-weight: 600;
  }

  .topic {
    color: var(--global-text-color, #0f172a);
  }

  .role-note {
    color: var(--global-text-color-light, #64748b);
    font-size: 0.82rem !important;
    font-style: italic;
  }

  .card-links {
    margin-top: 0.85rem;
  }

  .card-links a {
    display: inline-block;
    margin-right: 0.9rem;
    font-size: 0.84rem;
    font-weight: 700;
    text-decoration: none;
  }

  .card-links a:hover {
    text-decoration: underline;
  }

  @media (max-width: 768px) {
    .repsai-hero {
      grid-template-columns: 1fr;
      padding: 2rem 1.25rem;
    }

    .repsai-logo-wrap {
      order: -1;
      text-align: left;
    }

    .repsai-logo {
      width: 160px;
      max-width: 160px;
    }

    .member-grid,
    .repsai-card-grid {
      grid-template-columns: 1fr;
    }
  }
</style>


<!-- ========= HERO ========= -->
<div class="repsai-hero">

  <div class="repsai-hero-text">
    <div class="repsai-kicker">Representational AI Lab</div>

    <h1>Learning AI systems that adapt, align, and evolve reliably.</h1>

    <p class="repsai-subtitle">
      RepsAI focuses on machine learning methods for building adaptive, aligned, and trustworthy AI systems
      through representation learning, generative modeling, optimization, and continual learning.
    </p>

    <a href="/publications/" class="repsai-button">Publications</a>
  </div>
  </div>

  <div class="repsai-logo-wrap">
    <img src="{{ '/assets/img/repsai_lab.png' | relative_url }}" alt="RepsAI Lab" class="repsai-logo">
  </div>



<!-- ========= ABOUT ========= -->

## About the Lab

The **Representational AI Lab (RepsAI)** focuses on machine learning methods for building AI systems that can **adapt to new data and tasks**, **align with desired representations and objectives**, and **update their knowledge in a controlled and trustworthy way**.

Our work sits at the intersection of **representation learning**, **generative modeling**, **optimization**, **continual learning**, and **agentic AI**. We are particularly interested in how representations can make modern AI systems more **robust**, **controllable**, **efficient**, and **trustworthy**.

Applications of our work include inverse problems, scientific AI, computational pathology, foundation model adaptation, diffusion and flow-based generative models, and LLM agents.

<!-- ========= RESEARCH THEMES ========= -->

<div class="repsai-section">
  <h2>Research Themes</h2>
</div>

<div class="repsai-card-grid">

  <div class="repsai-topic-card">
    <div class="repsai-icon">🧠</div>
    <h3>Representation Learning</h3>
    <p>
      Learning structured, robust, and transferable representations that support adaptation,
      alignment, and reliable generalization.
    </p>
  </div>

  <div class="repsai-topic-card">
    <div class="repsai-icon">✨</div>
    <h3>Generative Models</h3>
    <p>
      Diffusion, flow-based, and latent-variable models for inverse problems, scientific AI,
      and controllable generation.
    </p>
  </div>

  <div class="repsai-topic-card">
    <div class="repsai-icon">⚙️</div>
    <h3>Optimization & Inference</h3>
    <p>
      Optimization, probabilistic inference, and theory for scalable, efficient, and reliable
      learning systems.
    </p>
  </div>

  <div class="repsai-topic-card">
    <div class="repsai-icon">🤖</div>
    <h3>Agentic & Continual AI</h3>
    <p>
      Adaptation, alignment, post-training, unlearning, and continual-learning methods for
      foundation models and LLM agents.
    </p>
  </div>

</div>


<!-- ========= CURRENT MEMBERS ========= -->

## Current Members

### PhD Students

<div class="member-grid">

  <div class="member-card phd-card">
    <div class="member-label">PhD Student</div>
    <h3>Loukas Sfountouris</h3>
    <p class="years">2024 – present</p>
    <p class="topic">Deep Generative Models</p>
    <p class="role-note">Main supervisor: Paris Giampouras · Co-supervisor: Prof. Theo Damoulas</p>
    <p class="card-links">
      <a href="#" target="_blank" rel="noopener"><i class="fas fa-globe"></i> Website</a>
      <a href="mailto:loukas.sfountouris@warwick.ac.uk"><i class="fas fa-envelope"></i> Email</a>
    </p>
  </div>

  <div class="member-card phd-card">
    <div class="member-label">PhD Student</div>
    <h3>Xietao Wang Li</h3>
    <p class="years">2024 – present</p>
    <p class="topic">AI/ML for Science</p>
    <p class="role-note">Co-supervisor: Paris Giampouras · Main supervisor: Prof. Tom Montenegro-Johnson</p>
    <p class="card-links">
      <a href="https://warwick.ac.uk/fac/sci/mathsys/people/students/mathsysii/wanglin/" target="_blank" rel="noopener"><i class="fas fa-globe"></i> Website</a>
      <a href="mailto:xietao.wang-lin@warwick.ac.uk"><i class="fas fa-envelope"></i> Email</a>
    </p>
  </div>

</div>

### Summer Interns

<div class="member-grid">

  <div class="member-card intern-card">
    <div class="member-label">Summer Intern</div>
    <h3>Liam Dalziel</h3>
    <p class="years">Warwick Mathematics Institute · 2026</p>
    <p class="topic">Continual Reinforcement Learning</p>
  </div>

  <div class="member-card intern-card">
    <div class="member-label">Summer Intern</div>
    <h3>Yikuan Li</h3>
    <p class="years">Warwick Mathematics Institute · 2026</p>
    <p class="topic">Posttraining of Diffusion Language Models</p>
  </div>

  <div class="member-card intern-card">
    <div class="member-label">Summer Intern</div>
    <h3>Yongqi Su</h3>
    <p class="years">Warwick Mathematics Institute · 2026</p>
    <p class="topic">Posttraining of Diffusion Language Models</p>
  </div>

  <div class="member-card intern-card">
    <div class="member-label">Summer Intern</div>
    <h3>Rong Rizheng</h3>
    <p class="years">Warwick Mathematics Institute · 2026</p>
    <p class="topic">Posttraining of Diffusion Language Models</p>
  </div>

  <div class="member-card intern-card">
    <div class="member-label">Summer Intern</div>
    <h3>Xiaoyu Gu</h3>
    <p class="years">Warwick Mathematics Institute · 2026</p>
    <p class="topic">Posttraining of Diffusion Language Models</p>
  </div>

</div>

### External Collaborators

<div class="member-grid">

  <div class="member-card external-card">
    <div class="member-label">External Collaborator</div>
    <h3>Omar Khamis Sayed Ahmed Allam</h3>
    <p class="years">AIMS · 2025 – present</p>
    <p class="topic">Dynamic Alignment of Large Language Models</p>
  </div>

</div>

<!-- ========= PAST MEMBERS ========= -->

## Past Members / Alumni

### MSc Dissertation Students

<div class="member-grid">

  <div class="member-card msc-card">
    <div class="member-label">MSc Dissertation</div>
    <h3>Byron Morris</h3>
    <p class="years">2025</p>
    <p class="topic">Generalized Counterfactuals for Image Generation in Computational Pathology</p>
  </div>

  <div class="member-card msc-card">
    <div class="member-label">MSc Dissertation</div>
    <h3>Razan Albalawi</h3>
    <p class="years">2025</p>
    <p class="topic">Semantic Defenses Against Adversarial Attacks Using Deep Generative Models</p>
  </div>

  <div class="member-card msc-card">
    <div class="member-label">MSc Dissertation</div>
    <h3>Sitthichai Charoensuk</h3>
    <p class="years">2025</p>
    <p class="topic">Machine Learning for Energy Prediction</p>
  </div>

</div>

### Past Interns

<div class="member-grid">

  <div class="member-card alumni-card">
    <div class="member-label">URSS Intern</div>
    <h3>Jake Barton Salazar</h3>
    <p class="years">BSc DCS · 2025</p>
    <p class="topic">Parameter-Efficient Fine-Tuning of Foundation Models</p>
    <p class="role-note">Co-supervised with Prof. Clarice Poon</p>
  </div>

  <div class="member-card alumni-card">
    <div class="member-label">URSS Intern</div>
    <h3>Thomas Yu</h3>
    <p class="years">BSc Mathematics · 2025</p>
    <p class="topic">Parameter-Efficient Fine-Tuning of Foundation Models</p>
    <p class="role-note">Co-supervised with Prof. Clarice Poon</p>
  </div>

  <div class="member-card alumni-card">
    <div class="member-label">URSS Intern</div>
    <h3>Hongxin Zhen</h3>
    <p class="years">BSc Mathematics · 2025</p>
    <p class="topic">Deep Inverse Problems</p>
    <p class="role-note">Co-supervised with Prof. Clarice Poon</p>
  </div>

  <div class="member-card alumni-card">
    <div class="member-label">URSS Intern</div>
    <h3>Toby Williams</h3>
    <p class="years">BSc Mathematics · 2025</p>
    <p class="topic">Deep Inverse Problems</p>
    <p class="role-note">Co-supervised with Prof. Clarice Poon</p>
  </div>

</div>
