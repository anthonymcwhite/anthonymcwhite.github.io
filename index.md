---
layout: page
title: ""
permalink: /
---

<section class="home-hero hero-splash">
  <div class="home-hero-inner">
    <div class="home-hero-left">
      <div class="kicker">Data • Systems • Practical analytics</div>
      <h1>Building reporting systems people can trust.</h1>
      <p>
        I build durable reporting systems, automate messy workflows, and translate complex data into decisions people can act on.
        My work sits at the intersection of impact measurement, operations, and security fundamentals.
      </p>

      <div class="home-actions">
        <a class="btn primary" href="{{ "/projects/" | relative_url }}">Projects</a>
        <a class="btn" href="{{ "/credentials/" | relative_url }}">Credentials</a>
        <a class="btn" href="{{ "/writing/" | relative_url }}">Writing</a>
        <a class="btn" href="{{ "/contact/" | relative_url }}">Contact</a>
      </div>

      <div class="pills">
        <div class="pill">Impact & Reporting</div>
        <div class="pill">CRM / Data Governance</div>
        <div class="pill">Automation</div>
        <div class="pill">Dashboards</div>
      </div>
    </div>

    <div class="home-hero-right">
      <img class="avatar" src="{{ "/assets/img/avatar-circle-512.png" | relative_url }}" alt="Portrait">
      <div class="home-hero-meta">
        <div class="meta-row">
          <div class="meta-label">Focus</div>
          <div class="meta-value">Measurement • Systems • Automation</div>
        </div>
        <div class="meta-row">
          <div class="meta-label">Location</div>
          <div class="meta-value">Delaware (US)</div>
        </div>
        <div class="meta-row">
          <div class="meta-label">Strengths</div>
          <div class="meta-value">Clarity, documentation, repeatability</div>
        </div>
      </div>
    </div>
  </div>
</section>

<section class="home-section">
  <div class="section-head">
    <h2>Featured work</h2>
    <a class="section-link" href="{{ "/projects/" | relative_url }}">View all →</a>
  </div>

  <div class="feature-tiles">
    <a class="feature-tile" href="{{ "/projects/" | relative_url }}">
      <div class="feature-title">Workforce pipeline analytics</div>
      <div class="feature-desc">Milestones, retention, and outcome reporting with operational dashboards.</div>
      <div class="feature-foot">Case study →</div>
    </a>

    <a class="feature-tile" href="{{ "/projects/" | relative_url }}">
      <div class="feature-title">Data governance & admin systems</div>
      <div class="feature-desc">Validation, deduplication, standards, and documentation that prevents drift.</div>
      <div class="feature-foot">Case study →</div>
    </a>

    <a class="feature-tile" href="{{ "/projects/" | relative_url }}">
      <div class="feature-title">Automation & reporting workflows</div>
      <div class="feature-desc">Repeatable pipelines that reduce manual effort, errors, and cycle time.</div>
      <div class="feature-foot">Case study →</div>
    </a>
  </div>
</section>

<section class="home-section">
  <div class="section-head">
    <h2>Latest writing</h2>
    <a class="section-link" href="{{ "/writing/" | relative_url }}">Browse all →</a>
  </div>

  {% assign recent = site.posts | slice: 0, 4 %}
  {% if recent.size > 0 %}
    <div class="post-list">
      {% for post in recent %}
        <a class="post-row" href="{{ post.url | relative_url }}">
          <div class="post-row-title">{{ post.title }}</div>
          <div class="post-row-date">{{ post.date | date: "%b %d, %Y" }}</div>
        </a>
      {% endfor %}
    </div>
  {% else %}
    <p class="muted">Posts will appear here once you publish them.</p>
  {% endif %}
</section>

<section class="home-section">
  <div class="section-head">
    <h2>Credentials</h2>
    <a class="section-link" href="{{ "/credentials/" | relative_url }}">See details →</a>
  </div>

  <div class="badge-strip">
    <img src="{{ "/assets/img/badges/comptia-data-plus-256.png" | relative_url }}" alt="CompTIA Data+">
    <img src="{{ "/assets/img/badges/comptia-project-p
