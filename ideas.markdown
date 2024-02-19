---
layout: default
weight: 2
title: Ideas
permalink: /ideas/
categories: ideas
---

<h2 style="text-align: center;">Poems</h2>
{%- for post in site.categories.ideas -%}
  {{ post.content }}

  {% if post.stars %}
    <h2 style="text-align: center;">
      {% for star in (1..post.stars) %}
        *
      {% endfor %}
    </h2>
  {% endif %}
{%- endfor -%}
