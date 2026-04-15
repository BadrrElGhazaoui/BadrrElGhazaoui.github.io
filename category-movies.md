---
layout: page
title: "Movies"
permalink: /category/Movies/
---

<div class="post-list">
  {% for post in site.categories.Movies %}
    <div class="post-preview">
      <a href="{{ post.url }}">
        <h2 class="post-title">{{ post.title }}</h2>
        {% if post.subtitle %}
        <h3 class="post-subtitle">{{ post.subtitle }}</h3>
        {% endif %}
      </a>
      <p class="post-meta">
        Posted on {{ post.date | date: "%B %-d, %Y" }}
      </p>
      <div class="post-entry">
        {% if post.excerpt %}
          {{ post.excerpt | strip_html | truncatewords: 50 }}
        {% endif %}
        <a href="{{ post.url }}" class="post-read-more">[Read&nbsp;More]</a>
      </div>
    </div>
    <hr class="post-list-separator" />
  {% endfor %}
</div>
