---
layout: default
weight: 2
title: Ideas
permalink: /ideas/
categories: ideas
---

<h2 style="text-align: center;">Ideas</h2>
{% for post in site.categories.ideas %}
  <h2 style="text-align: center;">***</h2>
  {{ post.content }}

