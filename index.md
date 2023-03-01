---
title: All posts
layout: default.liquid
---
# All posts

{% for post in collections.posts.pages %}
## [{{ post.title }}]({{ post.permalink }})
<p class="published_date">
  Published {{ post.published_date | date: "%Y-%m-%d" | escape }}
</p>

{% endfor %}
