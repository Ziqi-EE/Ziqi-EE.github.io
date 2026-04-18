---
layout: page
title: Contact
permalink: /contact/
eyebrow: Contact
description: For research discussions, collaboration, or academic correspondence.
---

{% assign profile = site.data.profile %}

<div class="split">
  <div class="prose">
    <h2>{{ profile.name }}</h2>
    <p>{{ profile.role }}, {{ profile.department }}</p>
    <p>{{ profile.affiliation }} · {{ profile.location }}</p>
  </div>

  <dl class="fact-list">
    <div>
      <dt>Research</dt>
      <dd>Micro/Nano Devices</dd>
    </div>
    <div>
      <dt>Academic Home</dt>
      <dd>{{ site.url }}</dd>
    </div>
  </dl>
</div>
