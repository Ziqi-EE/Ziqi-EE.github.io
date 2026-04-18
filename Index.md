---
layout: home
title: Home
permalink: /
description: Academic homepage of Song Ziqi.
---

{% assign profile = site.data.profile %}

<section class="section section--white">
  <div class="container split">
    <div class="split-copy">
      <p class="section-kicker">About</p>
      <h2>Micro/nano devices, from structure to mechanism.</h2>
      <p>{{ profile.summary }}</p>
    </div>
    <dl class="fact-list">
      <div>
        <dt>Affiliation</dt>
        <dd>{{ profile.affiliation }}</dd>
      </div>
      <div>
        <dt>Department</dt>
        <dd>{{ profile.department }}</dd>
      </div>
      <div>
        <dt>Location</dt>
        <dd>{{ profile.location }}</dd>
      </div>
    </dl>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="section-header">
      <div>
        <p class="section-kicker">Research</p>
        <h2>Current Interests</h2>
        <p>Focused topics across device design, fabrication, transport behavior, and functional materials.</p>
      </div>
      <a class="button button--primary" href="{{ '/research/' | relative_url }}">View Research</a>
    </div>
    <div class="grid">
      {% for item in site.data.research limit:3 %}
        <article class="feature-card">
          <h3>{{ item.title }}</h3>
          <p>{{ item.summary }}</p>
          <ul class="tag-list">
            {% for tag in item.tags limit:3 %}
              <li>{{ tag }}</li>
            {% endfor %}
          </ul>
        </article>
      {% endfor %}
    </div>
  </div>
</section>

<section class="section section--white">
  <div class="container">
    <div class="section-header">
      <div>
        <p class="section-kicker">Publications</p>
        <h2>Selected Work</h2>
      </div>
      <a class="button button--primary" href="{{ '/publications/' | relative_url }}">View All</a>
    </div>
    <div class="media-list">
      {% for publication in site.data.publications limit:1 %}
        {% include publication-card.html %}
      {% endfor %}
    </div>
  </div>
</section>
