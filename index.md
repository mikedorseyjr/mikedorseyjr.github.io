---
layout: page
title: Rumniations
tagline: Some thoughts of mine
---
{% include JB/setup %}

My "posts list".

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

Fix a crapton of stuff!!!
