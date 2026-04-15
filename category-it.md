
### Updated `category-it.md` Code
Delete the contents of `category-it.md` and paste this:

```yaml
---
layout: page
title: "IT"
permalink: /category/IT/
---

<div class="post-list">
  {% for post in site.categories.IT %}
    <div class="post-preview">
      <!-- Show Image if it exists -->
      {% if post.image %}
        <a href="{{ post.url }}">
          <img src="{{ post.image }}" alt="Thumbnail" class="img-fluid" style="max-width: 100%; height: auto; max-height: 300px; object-fit: cover; margin-bottom: 15px; border-radius: 5px;">
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
