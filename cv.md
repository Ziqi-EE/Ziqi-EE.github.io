---
layout: page
title: CV
permalink: /cv/
eyebrow: Curriculum Vitae
description: A concise academic overview.
---

{% assign profile = site.data.profile %}

<div class="split">
  <div>
    <p class="section-kicker">Education</p>
    <ul class="timeline">
      {% for item in profile.education %}
        <li>
          <strong>{{ item.degree }}</strong>
          <span>{{ item.institution }} · {{ item.period }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>

  <div>
    <p class="section-kicker">Research Areas</p>
    <ul class="timeline">
      {% for item in site.data.research limit:5 %}
        <li>
          <strong>{{ item.title }}</strong>
          <span>{{ item.summary }}</span>
        </li>
      {% endfor %}
    </ul>
  </div>
</div>
