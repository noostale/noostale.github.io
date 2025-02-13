---
title: Blog
layout: page
description: Blog posts
---

List of blog posts:

{% for post in site.posts %}
<p>
  <a href="{{ post.url }}">{{ post.title }}</a>
  <br>
  <small>{{ post.date | date_to_string }}</small>
</p>
{% endfor %}
