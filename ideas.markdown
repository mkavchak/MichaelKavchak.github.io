---
layout: default
weight: 2
title: Ideas
permalink: /ideas/
categories: ideas
---

{%- for post in site.categories.ideas -%}
  <h2 style="text-align: center;">***</h2>
  {{ post.content }}
  <h2 style="text-align: center;">**</h2>
{%- endfor -%}
