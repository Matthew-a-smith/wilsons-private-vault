---
layout: home
permalink: /
permalink_name: /home
title: Matthews-Project-Vault
detail_image: assets\cover33.svg
---

# Welcome to My Website

Hello, I'm Matthew. Welcome to my personal site, a space where I write articles and share my projects. My field of study is cybersecurity, with a focus on encryption algorithms, IoT device security, and programming.

---

### Areas of Expertise

**Encryption Algorithms**
***- Diffie-Hellman, RSA, MD5, HTTPS, TLS***

**IoT Device Security**
***- TLS/SSL, Baselineing, Network segmentation***

**IDS (Intrusion Detection Systems)**
***- Snort++, Suricata***

**Programming**
***- Python, JavaScript, SQL, Ruby, C++***

Check out my [about me](/about_me) page for more information on my experience and qualifications.

---

## Latest Articles

<ul class="article-card">
  {% assign count = 0 %}
  {% for post in site.posts %}
    {% if count < 2 %}
      <li>
        <a href="{{ post.url }}" class="article-list">{{ post.title }}</a>
        <span class="post-meta article-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
      </li>
      {% assign count = count | plus: 1 %}
    {% endif %}
  {% endfor %}
</ul>

Explore my [articles](/article) page, where I share projects from my classes and insights into interesting cybersecurity fields.