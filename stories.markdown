---
layout: default
weight: 3
title: Stories
permalink: /stories/
categories: stories
---

<h2 style="text-align: center;">Stories</h2>
{%- for post in site.categories.stories -%}
  {{ post.content }}

  {%- if post.stars -%}
    <h2 style="text-align: center;">
      {% for star in (1..post.stars) %}
        *
      {% endfor %}
    </h2>
  {%- endif -%}
{%- endfor -%}
