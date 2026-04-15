---
layout: page
title: "IT Posts"
permalink: /category/IT/
---

<ul>
  {% for post in site.categories.IT %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
      <span class="date">{{ post.date | date: "%B %e, %Y" }}</span>
    </li>
  {% endfor %}
</ul>
