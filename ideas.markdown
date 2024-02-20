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
