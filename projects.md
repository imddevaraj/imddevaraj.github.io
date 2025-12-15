---
layout: default
title: Projects
permalink: /projects/
---

<div class="container" style="padding-top: 4rem;">
  <h1 class="section-title" style="margin-top: 0;">Strategic Initiatives</h1>
  <div class="projects-grid">
      {% for project in site.data.projects %}
      <a href="{{ project.url }}" class="project-card">
        <h3>{{ project.title }}</h3>
        <p>{{ project.description }}</p>
        <div class="project-tags">
          {% for tag in project.tags %}
          <span>{{ tag }}</span>
          {% endfor %}
        </div>
      </a>
      {% endfor %}
  </div>
</div>
