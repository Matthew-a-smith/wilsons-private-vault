---
layout: home
title: About Me
permalink_name: /home
title: Matthews-Project-Vault
detail_image: assets\home_screen_deatil_header.svg
---

Home Page
---



---

Check out my [about me](/about_me) page for more information on my experience and qualifications.

---

## Latest Projects

<ul class="post-list">
  {% assign count = 0 %}
  {% for post in site.posts %}
    {% if count < 1 %}
      <li class="article-card">
        <span class="post-meta">{{ post.date | date: "%b %-d, %Y" }}</span>
        <h2>{{ post.title | escape }}</h2>
        <div class="post-content">
        <p class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 30 }}</p>
        <a href="{{ post.url | relative_url }}" class="read-more">Read more →</a>
        </div>
      </li>
      {% assign count = count | plus: 1 %}
    {% endif %}
  {% endfor %}
</ul>

