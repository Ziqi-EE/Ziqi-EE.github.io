---
layout: page
title: Publications
permalink: /publications/
eyebrow: Publications and Patents
description: Selected papers and patents. Each item keeps a dedicated image area on the left for figures, covers, graphical abstracts, or patent drawings.
---

<div class="section-header">
  <div>
    <p class="section-kicker">Papers</p>
    <h2>Selected Publications</h2>
  </div>
</div>

<div class="media-list">
  {% for publication in site.data.publications %}
    {% include publication-card.html %}
  {% endfor %}
</div>

<div class="section-header section-header--spaced">
  <div>
    <p class="section-kicker">Patents</p>
    <h2>Patents</h2>
  </div>
</div>

<div class="media-list">
  {% for patent in site.data.patents %}
    {% include patent-card.html %}
  {% endfor %}
</div>
