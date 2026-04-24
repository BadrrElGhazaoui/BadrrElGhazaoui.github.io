---
layout: page
title: "Songs"
permalink: /category/songs/
---
<div class="post-list">
  {% for post in site.categories.songs %}
    <div class="post-preview">
      {% if post.image %}
        <a href="{{ post.url }}">
          <img src="{{ post.image }}" alt="{{ post.title }}" style="width: 100%; max-height: 300px; object-fit: cover; border-radius: 5px; margin-bottom: 20px;">
        </a>
      {% endif %}
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
