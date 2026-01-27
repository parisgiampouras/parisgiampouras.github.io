---
layout: page
title: projects
permalink: /projects/
description: Recent Projects (more projects soon to be added)
nav: true
nav_order: 2
display_categories: [research]
horizontal: false
---

<!-- pages/projects.md -->

<div class="projects-page">

  <!-- Header / Intro -->
  <header class="projects-hero">
    <div class="projects-hero__text">
      <h1 class="projects-hero__title">Projects</h1>
      <p class="projects-hero__subtitle">
        A curated list of ongoing and recent research projects. For the full paper list, see:
      </p>

      <div class="projects-links">
        <a class="projects-link" href="{{ '/publications/' | relative_url }}">Publications</a>
        <a class="projects-link" href="https://scholar.google.com/citations?user=mZCc1TEAAAAJ" target="_blank" rel="noopener">Google Scholar</a>
        <a class="projects-link" href="https://arxiv.org/search/?searchtype=author&query=Giampouras%2C+P" target="_blank" rel="noopener">arXiv</a>
        <a class="projects-link" href="https://wrap.warwick.ac.uk/view/author_id/42640.default.html" target="_blank" rel="noopener">WRAP</a>
      </div>
    </div>
  </header>

  <!-- Projects -->
  <div class="projects">
    {%- if site.enable_project_categories and page.display_categories %}
      {%- for category in page.display_categories %}
        <h2 class="category">{{ category }}</h2>

        {%- assign categorized_projects = site.projects | where: "category", category -%}
        {%- assign sorted_projects = categorized_projects | sort: "importance" -%}

        {% if page.horizontal -%}
          <div class="container">
            <div class="row row-cols-2">
              {%- for project in sorted_projects -%}
                {% include projects_horizontal.html %}
              {%- endfor %}
            </div>
          </div>
        {%- else -%}
          <div class="grid projects-grid">
            {%- for project in sorted_projects -%}
              {% include projects.html %}
            {%- endfor %}
          </div>
        {%- endif -%}

      {% endfor %}
    {%- else -%}

      {%- assign sorted_projects = site.projects | sort: "importance" -%}

      {% if page.horizontal -%}
        <div class="container">
          <div class="row row-cols-2">
            {%- for project in sorted_projects -%}
              {% include projects_horizontal.html %}
            {%- endfor %}
          </div>
        </div>
      {%- else -%}
        <div class="grid projects-grid">
          {%- for project in sorted_projects -%}
            {% include projects.html %}
          {%- endfor %}
        </div>
      {%- endif -%}

    {%- endif -%}
  </div>

</div>

<style>
/* ---------- Layout ---------- */
.projects-page {
  margin-top: 0.5rem;
}

.projects-hero {
  border: 1px solid rgba(0,0,0,0.08);
  border-radius: 14px;
  padding: 1.1rem 1.2rem;
  margin: 0 0 1.25rem 0;
  background: rgba(0,0,0,0.02);
}

.projects-hero__title {
  margin: 0 0 0.25rem 0;
}

.projects-hero__subtitle {
  margin: 0.25rem 0 0.8rem 0;
  opacity: 0.85;
  line-height: 1.35;
}

.projects-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.55rem;
}

.projects-link {
  display: inline-flex;
  align-items: center;
  gap: 0.35rem;
  padding: 0.35rem 0.6rem;
  border-radius: 999px;
  border: 1px solid rgba(0,0,0,0.12);
  text-decoration: none !important;
  font-size: 0.92rem;
  background: white;
}

.projects-link:hover {
  transform: translateY(-1px);
  border-color: rgba(0,0,0,0.18);
}

/* ---------- Category header ---------- */
.projects h2.category {
  margin-top: 1.2rem;
  margin-bottom: 0.65rem;
}

/* ---------- Grid ---------- */
.projects-grid,
.projects .grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
  gap: 1.05rem;
}

/* ---------- Card polish (targets al-folio project cards) ---------- */
.projects .project {
  border-radius: 14px;
  overflow: hidden;
  border: 1px solid rgba(0,0,0,0.10);
  transition: transform 0.12s ease, box-shadow 0.12s ease, border-color 0.12s ease;
  background: white;
}

.projects .project:hover {
  transform: translateY(-2px);
  border-color: rgba(0,0,0,0.16);
  box-shadow: 0 8px 24px rgba(0,0,0,0.08);
}

/* ---------- Images: consistent sizing ---------- */
.projects .project img {
  width: 100%;
  max-width: none;          /* override prior 300px cap */
  height: 180px;            /* consistent card header height */
  object-fit: cover;        /* uniform crop */
  display: block;
}

/* If your template uses a wrapper around the image, keep it clean */
.projects .project .project-image,
.projects .project .card-img-top {
  margin: 0;
}

/* ---------- Mobile tweaks ---------- */
@media (max-width: 520px) {
  .projects-hero { padding: 0.95rem 0.95rem; }
  .projects .project img { height: 165px; }
}
</style>
