---
layout: page
title: Projects
permalink: /projects/
eyebrow: Projects
description: Research themes and project directions connected with micro/nano electronic devices.
---

<div class="grid">
  {% for project in site.data.projects %}
    <article class="project-card">
      <span class="status-pill">{{ project.status }}</span>
      <h3>{{ project.title }}</h3>
      <p>{{ project.summary }}</p>
    </article>
  {% endfor %}
</div>
