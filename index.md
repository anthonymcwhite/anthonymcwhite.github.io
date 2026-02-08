---
layout: page
title: ""
permalink: /
---

<div class="quicknav dossier-tabs">
  <a href="#top">Brief</a>
  <a href="#casefiles">Case Files</a>
  <a href="#writing">Field Notes</a>
  <a href="{{ "/credentials/" | relative_url }}">Credentials</a>
  <a href="{{ "/contact/" | relative_url }}">Contact</a>
</div>

<div id="top" class="hero dossier-hero">
  <div class="dossier-seal">
    <img src="{{ "/assets/img/brand/seal.png" | relative_url }}" alt="Seal">
  </div>

  <div class="card-grid">

    <div class="card half hero-splash dossier-brief">
      <div class="kicker">Operator Brief</div>
      <h1>Analytics systems that stay reliable when things get messy.</h1>

      <p>
        I build durable reporting systems, automate workflow friction, and translate complex data into decisions people can act on.
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
        <a class="cta" href="#casefiles">Open case files ↓</a>
        <a class="cta" href="{{ "/projects/" | relative_url }}">All projects →</a>
        <a class="cta" href="{{ "/writing/" | relative_url }}">Writing →</a>
      </div>

      <div class="dossier-meta">
        <div><span class="tag">Status</span> Active</div>
        <div><span class="tag">Focus</span> Systems • Measurement • Automation</div>
      </div>
    </div>

    <div class="card half dossier-profile">
      <div class="kicker">Profile</div>

      <div class="profile-row">
        <img class="headshot" src="{{ "/assets/img/headshot.jpg" | relative_url }}" alt="Headshot">

        <div class="profile-text">
          <p style="margin:0 0 8px 0;"><strong>What teams rely on me for</strong></p>
          <ul class="mini-list">
            <li>Turning messy data into stable metrics</li>
            <li>Governance + validation that prevents reporting drift</li>
            <li>Automation that reduces manual effort and error</li>
          </ul>

          <div class="cta-row" style="margin-top:12px;">
            <a class="cta" href="{{ "/credentials/" | relative_url }}">Credentials</a>
            <a class="cta" href="{{ "/contact/" | relative_url }}">Contact</a>
          </div>

          <p class="small-muted" style="margin-top:10px;">
            Delaware • open to analytics, operations, and systems-focused roles.
          </p>
        </div>
      </div>
    </div>

    <div id="casefiles" class="card">
      <div class="kicker">Case Files</div>
      <p class="small-muted" style="margin-top:8px;">
        Selected work themes—each becomes a case study as I publish more.
      </p>

      <div class="card-grid" style="margin-top:12px;">
        <a class="tile third dossier-tile" href="{{ "/projects/" | relative_url }}">
          <div class="tile-top">
            <span class="tile-code">CASE 01</span>
            <span class="tile-chip">Impact</span>
          </div>
          <p><strong>Workforce pipeline analytics</strong><br>
            <span class="small-muted">Milestones, retention, employer outcomes.</span>
          </p>
          <p class="small-muted">Open →</p>
        </a>

        <a class="tile third dossier-tile" href="{{ "/projects/" | relative_url }}">
          <div class="tile-top">
            <span class="tile-code">CASE 02</span>
            <span class="tile-chip">Governance</span>
          </div>
          <p><strong>Data governance & admin systems</strong><br>
            <span class="small-muted">Validation, deduplication, configuration standards.</span>
          </p>
          <p class="small-muted">Open →</p>
        </a>

        <a class="tile third dossier-tile" href="{{ "/projects/" | relative_url }}">
          <div class="tile-top">
            <span class="tile-code">CASE 03</span>
            <span class="tile-chip">Automation</span>
          </div>
          <p><strong>Automation & reporting workflows</strong><br>
            <span class="small-muted">Repeatable pipelines, less manual work.</span>
          </p>
          <p class="small-muted">Open →</p>
        </a>
      </div>
    </div>

    <div id="writing" class="card half">
      <div class="kicker">Field Notes</div>

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
        <p style="margin-top:12px;"><a href="{{ "/writing/" | relative_url }}">Browse all notes →</a></p>
      {% else %}
        <p class="small-muted" style="margin-top:10px;">Posts will appear here once you publish them.</p>
      {% endif %}
    </div>

    <div class="card half">
      <div class="kicker">Credentials Preview</div>
      <p class="small-muted" style="margin-top:10px;">
        Selected certifications and badges.
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
