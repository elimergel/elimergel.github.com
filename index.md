---
layout: page
title: Pinchers Of Power
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <span><h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a> </h2> &raquo;{{ post.date | date_to_string }}</span>
    {{ post.content }}
  {% endfor %}  
</ul>
