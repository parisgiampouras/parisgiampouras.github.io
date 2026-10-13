---
layout: page
title: Projects
permalink: /projects/
description: Foundations and algorithms for reliable, adaptive AI.
nav: true
nav_order: 2
display_categories: [research]
horizontal: false
---

<div class="projects-page">
  <div class="projects-hero">
    <p class="projects-hero__subtitle">
      My research connects optimization and structured representations with
      generative-model alignment, continual adaptation, causal inference,
      and AI research agents. Explore the projects below or browse the full publication list.
    </p>
    <div class="projects-links">
      <a class="projects-link" href="{{ '/publications/' | relative_url }}">Publications</a>
      <a class="projects-link" href="https://scholar.google.com/citations?user=mZCc1TEAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
      <a class="projects-link" href="https://arxiv.org/search/?searchtype=author&query=Giampouras%2C+P" target="_blank" rel="noopener">arXiv</a>
      <a class="projects-link" href="https://wrap.warwick.ac.uk/view/author_id/42640.default.html" target="_blank" rel="noopener">WRAP</a>
      <a class="projects-link" href="{{ '/repsai/' | relative_url }}">RAISE Lab</a>
    </div>
  </div>

  {%- if site.enable_project_categories and page.display_categories %}
    {%- for category in page.display_categories %}
      {%- assign categorized_projects = site.projects | where: "category", category -%}
      {%- assign sorted_projects = categorized_projects | sort: "importance" -%}
      <div class="projects-grid">
        {%- for project in sorted_projects %}
          {% include research_project_card.html %}
        {%- endfor %}
      </div>
    {%- endfor %}
  {%- else %}
    {%- assign sorted_projects = site.projects | sort: "importance" -%}
    <div class="projects-grid">
      {%- for project in sorted_projects %}
        {% include research_project_card.html %}
      {%- endfor %}
    </div>
  {%- endif %}
</div>

<style>
.projects-hero {
  border: 1px solid rgba(128, 128, 128, 0.2);
  border-radius: 14px;
  padding: 1.1rem 1.2rem;
  margin-bottom: 1.4rem;
  background: rgba(128, 128, 128, 0.04);
}
.projects-hero__subtitle {
  margin: 0 0 0.9rem;
  line-height: 1.6;
}
.projects-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
}
.projects-link {
  padding: 0.35rem 0.7rem;
  border: 1px solid rgba(128, 128, 128, 0.25);
  border-radius: 999px;
  color: var(--global-text-color);
  text-decoration: none;
  font-size: 0.92rem;
}
.projects-link:hover {
  border-color: var(--global-theme-color);
  color: var(--global-theme-color);
  text-decoration: none;
}
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
  gap: 1.2rem;
}
.research-project-card {
  overflow: hidden;
  border: 1px solid rgba(128, 128, 128, 0.22);
  border-radius: 14px;
  background: var(--global-bg-color);
  transition: transform 0.15s ease, box-shadow 0.15s ease;
}
.research-project-card:hover {
  transform: translateY(-3px);
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.1);
}
.research-project-card__link {
  display: flex;
  flex-direction: column;
  height: 100%;
  color: var(--global-text-color);
  text-decoration: none;
}
.research-project-card__link:hover {
  color: var(--global-text-color);
  text-decoration: none;
}
.research-project-card__link:focus-visible {
  outline: 3px solid var(--global-theme-color);
  outline-offset: -3px;
}
.research-project-card__image {
  background: #f7f5fb;
}
.research-project-card__image figure {
  margin: 0;
}
.research-project-card__image img {
  display: block;
  width: 100%;
  max-width: none;
  height: 175px;
  object-fit: contain;
}
.research-project-card__body {
  display: flex;
  flex-direction: column;
  flex: 1;
  padding: 1.1rem;
}
.research-project-card__title {
  margin: 0 0 0.65rem;
  font-size: 1.15rem;
  line-height: 1.35;
}
.research-project-card__description {
  margin-bottom: 1rem;
  font-size: 0.95rem;
  line-height: 1.5;
}
.research-project-card__more {
  margin-top: auto;
  color: var(--global-theme-color);
  font-size: 0.9rem;
}
@media (max-width: 520px) {
  .projects-grid { grid-template-columns: 1fr; }
  .projects-hero { padding: 1rem; }
}
</style>
