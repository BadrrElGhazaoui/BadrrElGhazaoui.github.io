---
layout: page
title: "IT Posts"
permalink: /category/IT/
---

<!-- 1. Grab only the posts that belong to the 'IT' category -->
{% assign filtered_posts = site.categories.IT %}

<!-- 2. Display them using the Beautiful Jekyll layout -->
{% include list-posts.html posts=filtered_posts %}
