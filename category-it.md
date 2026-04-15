---
layout: page
title: "IT Posts"
permalink: /category/IT/
---

<div class="row">
  {% for post in site.categories.IT %}
    <div class="col-sm-4">
      <div class="card h-100">
        <div class="card-header">
          <h4 class="post-title">
            <a class="post-link" href="{{ post.url }}">{{ post.title }}</a>
          </h4>
          <h5 class="post-date">{{ post.date | date: "%B %e, %Y" }}</h5>
        </div>
        <div class="card-body">
          <p class="card-text">
            {% if post.excerpt %}
              {{ post.excerpt | strip_html | truncatewords: 50 }}
            {% else %}
              No content provided.
            {% endif %}
          </p>
        </div>
        <div class="card-footer bg-white border-top-0">
          <a href="{{ post.url }}" class="btn btn-primary">Read More</a>
        </div>
      </div>
    </div>
  {% endfor %}
</div>
