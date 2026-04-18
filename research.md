---
layout: page
title: Research
permalink: /research/
eyebrow: Research
description: Research interests across micro/nano devices, device physics, molecular electronics, and functional electronic materials.
---

<div class="grid">
  {% for item in site.data.research %}
    <article class="feature-card">
      <h3>{{ item.title }}</h3>
      <p>{{ item.summary }}</p>
      <ul class="tag-list">
        {% for tag in item.tags %}
          <li>{{ tag }}</li>
        {% endfor %}
      </ul>
    </article>
  {% endfor %}
</div>
