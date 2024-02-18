---
layout: default
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
