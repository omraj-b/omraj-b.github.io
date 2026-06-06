---
layout: default
title: Home
---

<div class="container hero">

<div class="about-text">

  <h1>Hi, I'm Omraj</h1>
  <h2 class="subtitle">Aspiring Cybersecurity Analyst</h2>

  <div class="card about-card">
  
    <p>
      My journey into cybersecurity started with curiosity—and quickly turned into a structured, hands-on pursuit of understanding how systems work and how they break.
    </p>

    <p>
      Over the past year, I have focused on building a strong foundation in cybersecurity through a combination of theory and practical labs. I completed the CompTIA Security+ and CCNA syllabi, and consistently applied those concepts through hands-on work using platforms like TryHackMe, where I have solved 50+ labs across domains such as SOC operations, Active Directory, cryptography, and network security.
    </p>

    <p>
      What defines my approach is learning by doing. I have built and experimented with multiple lab environments to simulate real-world scenarios:
    </p>

    <ul>
      <li>Capturing and analyzing network traffic using Wireshark to understand protocol behavior and detect anomalies</li>
      <li>Scanning and assessing vulnerable systems using Nmap and OpenVAS</li>
      <li>Setting up a virtual SOC lab with Wazuh to observe attacks from a defender’s perspective</li>
      <li>Practicing password security, hashing, and cracking techniques to understand authentication weaknesses</li>
      <li>Exploring web vulnerabilities through PortSwigger labs, including SQL injection and authentication bypass</li>
    </ul>

    <p>
      Along the way, I’ve also explored areas like malware behavior, system internals (Windows/Linux), and basic Active Directory concepts to understand how attackers exploit real systems.
    </p>

    <p>
      Currently, I am focused on improving my web application security skills, working through PortSwigger labs, attempting CTF challenges, and gradually stepping into bug bounty programs to gain exposure to real-world security testing.
    </p>

    <p>
      Before transitioning into cybersecurity, I completed my M.Tech from IIT Bombay, where I worked as a Teaching Assistant in courses involving GNU Radio and RFID-based system design. I also led the Fine Arts Club during my undergraduate studies at IIT Ropar, an experience that taught me how creativity and structured thinking can complement each other—something I still apply in problem-solving today.
    </p>

    <p>
      I am now looking for opportunities where I can contribute as a cybersecurity analyst while continuing to learn, build, and refine my skills in a practical environment.
    </p>

  </div>

  <div class="cta">
    <a class="btn" href="/blog">Read Blog</a>
    <a class="btn secondary" href="/resume">View Resume</a>
  </div>

</div>

<div class="about-image">
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