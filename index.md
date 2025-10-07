---
layout: default
description: Home page of Emanuele Frasca's personal website
updated_at: "2025-07-10"
---

Hi, I'm Emanuele.

I'm a computer engineer from Italy, currently pursuing a master's degree in *Artificial Intelligence and Robotics* at *Sapienza University of Rome*.

My main interests lie in:
- Representation Learning
- Natural Language Processing
- Deep Reinforcement Learning

Check out my projects on [GitHub](https://github.com/noostale), or connect with me on [LinkedIn](https://www.linkedin.com/in/emanuelefrasca/).  
You can also reach me via email at <a href="mailto:emanuele&#46;frasca&#46;00&#64;gmail&#46;com">emanuele.frasca.00@gmail.com</a>

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