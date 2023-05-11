---
layout: page
title: Projects
permalink: /projects/
description: Recent Projects (more projects soon to be added)
nav: true
nav_order: 2
display_categories: [research]
horizontal: false
---

<!-- pages/projects.md -->

<style>
.projects {
  margin: 50px 0;
}

.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(350px, 1fr));
  grid-gap: 40px;
  margin: 0 auto;
  max-width: 1200px;
}

.card {
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
  padding: 20px;
  transition: all 0.3s ease;
}

.card:hover {
  transform: translateY(-10px);
}

.card h3 {
  font-size: 24px;
  margin-top: 0;
}

.card p {
  font-size: 16px;
  line-height: 1.5;
  margin-bottom: 20px;
}

.card img {
  max-width: 100%;
  height: auto;
  margin-bottom: 20px;
}

.category {
  font-size: 32px;
  font-weight: bold;
  margin-bottom: 40px;
}

@media only screen and (max-width: 768px) {
  .grid {
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  }
}
</style>

<div class="projects">
{%- if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {%- for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
  {%- assign categorized_projects = site.projects | where: "category", category -%}
  {%- assign sorted_projects = categorized_projects | sort: "importance" %}
  <!-- Generate cards for each project -->
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
  {% endfor %}

{%- else -%}
<!-- Display projects without categories -->
  {%- assign sorted_projects = site.projects | sort: "importance" -%}
  <!-- Generate cards for each project -->
  <div class="grid">
    {%- for project in sorted_projects -%}
      {% include projects.html %}
    {%- endfor %}
  </div>
{%- endif -%}
</div>
