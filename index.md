---
layout: page
title: ""
permalink: /
---

<!-- Sticky quick-nav -->
<div class="quicknav">
  <a href="#top">Top</a>
  <a href="#work">Work</a>
  <a href="#writing">Writing</a>
  <a href="{{ "/credentials/" | relative_url }}">Credentials</a>
  <a href="{{ "/contact/" | relative_url }}">Contact</a>
</div>

<div id="top" class="hero">
  <div class="card-grid">

    <!-- HERO SPLASH -->
    <div class="card half hero-splash">
      <div class="kicker">Data • Systems • Security-minded analytics</div>

      <!-- Role-first headline (no name) -->
      <h1>Analytics + operations systems that hold up under pressure.</h1>

      <p>
        I build durable reporting systems, automate messy workflows, and translate complex data into decisions people can act on.
        My work sits at the intersection of impact measurement, operations, and practical security.
      </p>

      <div class="pills">
        <div class="pill">Impact & Reporting</div>
        <div class="pill">CRM / Data Governance</div>
        <div class="pill">Automation</div>
        <div class="pill">Dashboards</div>
        <div class="pill">Security fundamentals</div>
      </div>

      <div class="cta-row">
        <a class="cta" href="#work">Explore work ↓</a>
        <a class="cta" href="{{ "/projects/" | relative_url }}">Projects →</a>
        <a class="cta" href="{{ "/writing/" | relative_url }}">Writing →</a>
        <a class="cta" href="{{ "/contact/" | relative_url }}">Contact →</a>
      </div>

      <p class="small-muted" style="margin-top:10px;">
        Professional portfolio here • deeper builds and experiments live on <span style="color:var(--text);">civint.tech</span>
      </p>
    </div>

    <!-- PROFILE -->
    <div class="card half">
      <div class="kicker">Profile</div>

      <div style="display:flex; gap:16px; align-items:flex-start; flex-wrap:wrap;">
        <img class="headshot" src="{{ "/assets/img/headshot.jpg" | relative_url }}" alt="Headshot">
        <div style="min-width:240px; flex:1;">
          <p style="margin:0 0 8px 0;"><strong>What I’m known for</strong></p>
          <ul class="mini-list">
            <li>Turning messy data into reliable metrics</li>
            <li>Building repeatable reporting + governance</li>
            <li>Automation that reduces manual effort</li>
          </ul>

          <div class="cta-row" style="margin-top:12px;">
            <a class="cta" href="{{ "/credentials/" | relative_url }}">Credentials</a>
            <a class="cta" href="{{ "/contact/" | relative_url }}">Contact</a>
          </div>
        </div>
      </div>
    </div>

    <!-- FEATURED WORK (clickable cards) -->
    <div id="work" class="card">
      <div class="kicker">Featured work</div>

      <div class="card-grid" style="margin-top:10px;">
        <a class="card third clickable" href="{{ "/projects/" | relative_url }}">
          <p><strong>Workforce pipeline analytics</strong><br>
            <span class="small-muted">Milestones, retention, employer outcomes.</span>
          </p>
          <p class="small-muted">View →</p>
        </a>

        <a class="card third clickable" href="{{ "/projects/" | relative_url }}">
          <p><strong>Data governance & admin systems</strong><br>
            <span class="small-muted">Validation, deduplication, configuration standards.</span>
          </p>
          <p class="small-muted">View →</p>
        </a>

        <a class="card third clickable" href="{{ "/projects/" | relative_url }}">
          <p><strong>Automation & reporting workflows</strong><br>
            <span class="small-muted">Repeatable pipelines, less manual work.</span>
          </p>
          <p class="small-muted">View →</p>
        </a>
      </div>
    </div>

    <!-- LATEST WRITING (dynamic) -->
    <div id="writing" class="card half">
      <div class="kicker">Latest writing</div>

      {% assign recent = site.posts | slice: 0, 3 %}
      {% if recent.size > 0 %}
        <div style="margin-top:10px;">
          {% for post in recent %}
            <div style="padding:12px 0; border-top: 1px solid var(--border);">
              <div style="display:flex; justify-content:space-between; gap:12px; flex-wrap:wrap;">
                <a href="{{ post.url | relative_url }}"><strong>{{ post.title }}</strong></a>
                <span class="small-muted">{{ post.date | date: "%b %d, %Y" }}</span>
              </div>
              {% if post.excerpt %}
                <div class="small-muted" style="margin-top:6px;">{{ post.excerpt | strip_html | truncate: 140 }}</div>
              {% endif %}
            </div>
          {% endfor %}
        </div>
        <p style="margin-top:12px;"><a href="{{ "/writing/" | relative_url }}">Browse all writing →</a></p>
      {% else %}
        <p class="small-muted" style="margin-top:10px;">Posts will appear here once you publish them.</p>
      {% endif %}
    </div>

    <!-- CREDENTIALS PREVIEW -->
    <div class="card half">
      <div class="kicker">Credentials</div>
      <p class="small-muted" style="margin-top:10px;">
        Selected certifications and badges — built for credibility, not clutter.
      </p>

      <div style="display:flex; flex-wrap:wrap; gap:10px; margin-top:10px;">
        <img style="height:44px; width:auto;" src="{{ "/assets/img/badges/comptia-data-plus-256.png" | relative_url }}" alt="CompTIA Data+">
        <img style="height:44px; width:auto;" src="{{ "/assets/img/badges/comptia-project-plus-256.png" | relative_url }}" alt="CompTIA Project+">
        <img style="height:44px; width:auto;" src="{{ "/assets/img/badges/google-cybersecurity-256.png" | relative_url }}" alt="Google Cybersecurity">
        <img style="height:44px; width:auto;" src="{{ "/assets/img/badges/bonterra-apricot-certified-admin-256.png" | relative_url }}" alt="Apricot Admin">
      </div>

      <p style="margin-top:12px;">
        <a href="{{ "/credentials/" | relative_url }}">View credentials →</a>
      </p>
    </div>

  </div>
</div>
