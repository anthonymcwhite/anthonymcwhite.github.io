---
layout: page
title: Notebook
permalink: /writing/
---

<div class="page-lead">
  <div class="section-label">Notebook / Field records</div>
  <h1>Observations from inside the system.</h1>
  <p>Short writing, project decisions, technical findings, and longer reflections from professional practice and the workbench. Entries distinguish firsthand experience from interpretation and link to supporting material wherever it can be shared responsibly.</p>
</div>

<div class="post-index">
{% for post in site.posts %}
  <a class="post-entry" href="{{ post.url | relative_url }}">
    <span>{{ post.date | date: "%Y.%m.%d" }}</span>
    <strong>{{ post.title }}</strong>
    <em>Read note →</em>
  </a>
{% endfor %}
</div>

## Forthcoming threads

- **Listen First** — the beginning of my radio journey
- **Building a field console** — a headless Raspberry Pi system for the vehicle and field
- **Maintaining a community mesh** — devices, nodes, and Wilmington Meshtastic
- **What failed on the bench** — short records of useful mistakes
