---
layout: default
weight: 1
title: Poems
permalink: /poems/
categories: poems
---

# Poems:
{% for post in site.categories.poems %}
  <h2 style="text-align: center;">***</h2>
  {{ post.content }}
  <h2 style="text-align: center;">**</h2>
{% endfor %}
