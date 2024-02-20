---
layout: default
weight: 3
title: Stories
permalink: /stories/
categories: stories
---

<h2 style="text-align: center;">Stories</h2>
{%- for post in site.categories.stories -%}
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
