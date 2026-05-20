---
layout: default
title: Home
---

<div class="container hero">

<div>
  <h1>Cybersecurity Learner & Engineer</h1>
  <p>
    I am Omraj Burnwal, with a background in communication and signal processing,
    now transitioning into cybersecurity with hands-on experience in SIEM tools,
    SOC workflows, and system-level concepts.
  </p>

  <a class="btn" href="/blog">Explore Blog</a>
</div>

<div class="hero-box">
  <h3>Current Focus</h3>
  <ul>
    <li>Security+ Completed</li>
    <li>CCNA in progress</li>
    <li>Operating Systems</li>
    <li>SIEM: Splunk & Wazuh</li>
  </ul>
</div>

</div>

<div class="container section">
  <h2>Projects</h2>

  <div class="grid">
    <div class="card">
      <h3>SIEM Monitoring Lab</h3>
      <p>Configured Splunk and Wazuh for log ingestion, alerting, and analysis.</p>
    </div>

    <div class="card">
      <h3>Live SOC Practice</h3>
      <p>Performed alert triage and investigated simulated incidents.</p>
    </div>
  </div>
</div>

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