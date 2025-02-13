---
layout: default
---

Hello! My name is **Emanuele Frasca**. I'm from Rome, Italy.

I'm a computer engineer, currently studying Artificial Intelligence and Robotics at the University of Rome "La Sapienza".

List of blog posts:

{% for post in site.posts %}
<p>
  <a href="{{ post.url }}">{{ post.title }}</a>
  <br>
  <small>{{ post.date | date_to_string }}</small>
</p>
{% endfor %}