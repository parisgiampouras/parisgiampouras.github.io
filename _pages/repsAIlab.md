---
layout: page
title: RAISE Lab
nav: true
description: Reliable, Adaptive, and Self-Improving AI Lab
permalink: /repsai/
nav_order: 3
---

<style>
  /* ========= RAISE LAB PAGE ========= */

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

.raise-wordmark {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  width: 230px;
  height: 230px;
  margin-left: auto;
  border-radius: 1.25rem;
  color: #ffffff;
  background: linear-gradient(145deg, #1d4ed8 0%, #0284c7 100%);
  border: 4px solid rgba(255, 255, 255, 0.95);
  box-shadow: 0 14px 30px rgba(15, 23, 42, 0.16);
  font-size: 2.3rem;
  font-weight: 850;
  letter-spacing: -0.05em;
}

.raise-wordmark span {
  margin-top: 0.2rem;
  font-size: 0.78rem;
  font-weight: 750;
  letter-spacing: 0.28em;
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

    .raise-wordmark {
      width: 160px;
      height: 160px;
      margin-left: 0;
      font-size: 1.8rem;
    }

    .member-grid,
    .repsai-card-grid {
      grid-template-columns: 1fr;
    }
  }


  /* ========= DARK MODE FIXES ========= */

html[data-theme='dark'] .repsai-hero {
  background:
    radial-gradient(circle at top left, rgba(34, 211, 238, 0.14), transparent 34%),
    radial-gradient(circle at bottom right, rgba(59, 130, 246, 0.18), transparent 36%),
    linear-gradient(135deg, #18181b 0%, #111827 100%);
  border: 1px solid rgba(148, 163, 184, 0.22);
  box-shadow: 0 14px 36px rgba(0, 0, 0, 0.35);
}

html[data-theme='dark'] .repsai-kicker {
  color: var(--global-theme-color, #38bdf8);
  background: rgba(15, 23, 42, 0.78);
  border: 1px solid rgba(148, 163, 184, 0.24);
}

html[data-theme='dark'] .repsai-hero h1 {
  color: var(--global-text-color, #f8fafc);
}

html[data-theme='dark'] .repsai-subtitle {
  color: var(--global-text-color-light, #cbd5e1);
}

html[data-theme='dark'] .repsai-logo {
  border-color: rgba(15, 23, 42, 0.9);
  box-shadow: 0 16px 34px rgba(0, 0, 0, 0.38);
}

html[data-theme='dark'] .raise-wordmark {
  border-color: rgba(15, 23, 42, 0.9);
  box-shadow: 0 16px 34px rgba(0, 0, 0, 0.38);
}

html[data-theme='dark'] .repsai-topic-card,
html[data-theme='dark'] .member-card {
  background: var(--global-card-bg-color, #1f2937);
  border-color: rgba(148, 163, 184, 0.22);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.28);
}

html[data-theme='dark'] .repsai-topic-card:hover,
html[data-theme='dark'] .member-card:hover {
  border-color: rgba(56, 189, 248, 0.35);
  box-shadow: 0 14px 34px rgba(0, 0, 0, 0.38);
}

html[data-theme='dark'] .repsai-icon,
html[data-theme='dark'] .member-label {
  background: rgba(56, 189, 248, 0.12);
  color: var(--global-theme-color, #38bdf8);
}

html[data-theme='dark'] .topic {
  color: var(--global-text-color, #f8fafc);
}

html[data-theme='dark'] .years,
html[data-theme='dark'] .role-note,
html[data-theme='dark'] .repsai-topic-card p {
  color: var(--global-text-color-light, #cbd5e1);
}
</style>


<!-- ========= HERO ========= -->
<div class="repsai-hero">

  <div class="repsai-hero-text">
    <div class="repsai-kicker">Reliable · Adaptive · Self-Improving AI</div>

    <h1>Building robust, adaptive, and self-improving AI systems.</h1>

    <p class="repsai-subtitle">
      RAISE develops learning algorithms for generative models and agentic AI systems
      drawing on optimization, probabilistic inference, representation learning, and control.
    </p>

    <a href="/publications/" class="repsai-button">Publications</a>
  </div>

  <div class="repsai-logo-wrap">
    <div class="raise-wordmark" aria-label="RAISE Lab">
      RAISE
      <span>LAB</span>
    </div>
  </div>

</div>


<!-- ========= ABOUT ========= -->

## About the Lab

The **Reliable, Adaptive, and Self-Improving AI Lab (RAISE)** develops machine learning methods for AI systems that can **adapt to new tasks**, **learn from feedback**, and **improve their capabilities reliably over time**.

Our research spans three connected areas: **machine-learning foundations**, including optimization, probabilistic inference, representation learning, and control; **generative AI**, particularly diffusion and flow-based models; and **autonomous, self-improving AI**, including  test-time scaling, and continual adaptation.


<!-- ========= RESEARCH THEMES ========= -->

<div class="repsai-section">
  <h2>Research Themes</h2>
</div>

<div class="repsai-card-grid">

  <div class="repsai-topic-card">
    <div class="repsai-icon">⚙️</div>
    <h3>Foundations of Learning</h3>
    <p>
      Optimization, probabilistic inference, representation learning, and control for robust,
      efficient, and scalable learning systems.
    </p>
  </div>

  <div class="repsai-topic-card">
    <div class="repsai-icon">✨</div>
    <h3>Generative AI</h3>
    <p>
      Diffusion, flow-based, and latent-variable models for controllable generation,
      inverse problems, and scientific applications.
    </p>
  </div>

  <div class="repsai-topic-card">
    <div class="repsai-icon">🤖</div>
    <h3>Autonomous & Self-Improving AI</h3>
    <p>
       test-time scaling, and recursive self-improvement through
      exploration, memory, feedback, and continual adaptation.
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
