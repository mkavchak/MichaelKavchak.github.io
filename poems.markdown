---
layout: default
weight: 1
title: Poems
permalink: /poems/
categories: poems
---

<h2 style="text-align: center;">Poems</h2>
{%- for post in site.categories.poems -%}
  {{ post.content }}

  {%- if post.stars -%}
    <h2 style="text-align: center;">
      {% for star in (1..post.stars) %}
        *
      {% endfor %}
    </h2>
  {%- endif -%}
{%- endfor -%}
