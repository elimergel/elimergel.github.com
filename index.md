---
layout: page
title: index
---
{% include JB/setup %}

<ul class="posts">
  {% for post in site.posts %}
    <span><h2><a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a><small>     &raquo;{{ post.date | date_to_string }}</small></h2></span>
    {{ post.content }}
  {% endfor %}  
</ul>

{% if user %}
  Hello {{ user.name }}
{% endif %}
