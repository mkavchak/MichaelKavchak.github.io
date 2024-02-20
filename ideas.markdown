---
layout: default
weight: 2
title: Ideas
permalink: /ideas/
categories: ideas
---

<h2 style="text-align: center;">Ideas</h2>
{%- for post in site.categories.ideas -%}
  {% if post.categories contains 'delete' %}
    {%- continue -%}
  {% endif %}
  {%- if post.stars -%}
    <h2 style="text-align: center;">
      {% for star in (1..post.stars) %}
        *
      {% endfor %}
    </h2>
  {%- endif -%}
  {{ post.content }}
{%- endfor -%}
