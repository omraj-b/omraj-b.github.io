---
layout: default
title: Home
---

<div class="container hero">

<div>
  <h1>Hi, I'm Omraj</h1>
  <h2 class="subtitle">Cybersecurity Enthusiast</h2>

  <p>
    Transitioning from communication and signal processing into cybersecurity.
    Currently building hands-on experience with SIEM tools, networking, and system-level concepts.
  </p>

  <div class="cta">
    <a class="btn" href="/blog">Read Blog</a>
    <a class="btn secondary" href="/resume">View Resume</a>
  </div>
</div>

<div>
  <img src="/assets/images/profile.jpg" alt="Omraj Burnwal" class="profile-img">
</div>

</div>

<!-- SKILLS / FOCUS -->
<div class="container section">
  <h2>What I'm Focused On</h2>

  <div class="grid">
    <div class="card">
      <h3>SIEM & Monitoring</h3>
      <p>Working with Splunk and Wazuh for log ingestion, alerting, and analysis.</p>
    </div>

    <div class="card">
      <h3>Networking</h3>
      <p>Preparing for CCNA and building strong understanding of network fundamentals.</p>
    </div>

    <div class="card">
      <h3>Operating Systems</h3>
      <p>Learning processes, memory, and system-level behavior from a security perspective.</p>
    </div>
  </div>
</div>

<!-- PROJECTS -->
<div class="container section">
  <h2>Projects</h2>

  <div class="grid">
    <div class="card">
      <h3>SIEM Monitoring Lab</h3>
      <p>
        Configured Splunk and Wazuh to collect logs, create alerts,
        and analyze system activity.
      </p>
    </div>

    <div class="card">
      <h3>Live SOC Practice</h3>
      <p>
        Investigated alerts, performed triage, and analyzed simulated
        security incidents.
      </p>
    </div>
  </div>
</div>

<!-- BLOG -->
<div class="container section">
  <h2>Latest Blog Posts</h2>

  <div class="grid">
    {% for post in site.posts limit:3 %}
      <div class="card post-card">
        <h3><a href="{{ post.url }}">{{ post.title }}</a></h3>
        <p class="date">{{ post.date | date: "%b %d, %Y" }}</p>
        <p>{{ post.excerpt }}</p>
      </div>
    {% endfor %}
  </div>
</div>