---
layout: archive
title: "作品集"
permalink: /projects/
---

{% assign projects = site.projects | sort: "title" %}

<div class="project-grid">
  {% for project in projects %}
    <article class="project-card">
      <a href="{{ project.url | relative_url }}">
        {% if project.image %}
          <img src="{{ project.image | relative_url }}" alt="{{ project.title }}" loading="lazy">
        {% endif %}
      </a>
      <div class="project-body">
        <h3><a href="{{ project.url | relative_url }}">{{ project.title }}</a></h3>
        {% if project.excerpt %}
          <p>{{ project.excerpt }}</p>
        {% endif %}
      </div>
    </article>
  {% endfor %}
</div>

## 说明

这里是我的作品集入口，用来展示我感兴趣的内容和创作方向。后续我会继续替换为真实内容，完善每个作品的说明和作品链接。
