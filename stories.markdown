---
layout: default
weight: 3
title: Stories
permalink: /stories/
categories: stories
---

# Stories:
{% for post in site.categories.stories %}
  <h2 style="text-align: center;">***</h2>
  {{ post.content }}
  <h2 style="text-align: center;">**</h2>
{% endfor %}
