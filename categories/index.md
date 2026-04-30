---
layout: page
title: 分类
permalink: /categories/
---

# 📂 分类列表

{% for category in site.categories %}
## {{ category[0] }}

<ul>
  {% for post in category[1] %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>

{% endfor %}
