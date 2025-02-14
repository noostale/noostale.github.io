---
layout: default
description: Home page of Emanuele Frasca's personal website
updated_at: "2025-02-14"
---

Hi, I'm Emanuele.

I'm a computer engineer from Italy, currently studying *Artificial Intelligence and Robotics* at the *University of Rome "La Sapienza"*.

My main interests are in the fields of:
- Deep Learning
- Representation Learning
- Geometric Deep Learning
- Explainable AI
- Natural Language Processing
- Deep Reinforcement Learning

{% if site.posts.size > 0 %}
  ## List of blog posts
  {% for post in site.posts %}
  <p>
    <a href="{{ post.url }}">{{ post.title }}</a>
    <br>
    <small>{{ post.date | date_to_string }}</small>
  </p>
  {% endfor %}

{% endif %}