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
  <div class="post-data">
    {%- if post.stars -%}
      <h2 class="stars-field">
        {% for star in (1..post.stars) %}
          *
        {% endfor %}
      </h2>
    {%- endif -%}
    {{ post.content }}
  </div>
{%- endfor -%}
