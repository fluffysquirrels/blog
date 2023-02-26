---
title: All posts
layout: default.liquid
---
# All posts

{% for post in collections.posts.pages %}
## [{{ post.title }}]({{ post.permalink }})
{% endfor %}
