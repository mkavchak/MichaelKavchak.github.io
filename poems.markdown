---
layout: default
weight: 1
title: Poems
permalink: /poems/
categories: poems
---
# Poems:

{% for post in site.categories.poems %}
### {{ post.title }}
{{ post.date | date: "%B %d, %Y" }}

{{ post.content }}
{% endfor %}
