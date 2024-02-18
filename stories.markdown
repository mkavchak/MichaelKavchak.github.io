---
layout: default
weight: 3
title: Stories
permalink: /stories/
categories: stories
---
# Stories:

{% for post in site.categories.stories %}
### {{ post.title }}
{{ post.date | date: "%B %d, %Y" }}

{{ post.content }}
{% endfor %}
