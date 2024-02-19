---
layout: default
weight: 1
title: Poems
permalink: /poems/
categories: poems
---

<h2 style="text-align: center;">Poems</h2>
{%- for post in site.categories.poems -%}
  {% if post.categories contains 'delete' %}
    {%- continue -%}
  {% endif %}
  {{ post.content }}

  {%- if post.stars -%}
    <h2 style="text-align: center;">
      {% for star in (1..post.stars) %}
        *
      {% endfor %}
    </h2>
  {%- endif -%}
{%- endfor -%}
