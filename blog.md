---
layout: default
title: Blog
---



<ul>
  {% for post in site.posts %}
    <li>
      <a href="{{ post.url }}">{{ post.title }}</a>
    </li>
  {% endfor %}
</ul>


{% for post in site.posts %}
<h3>{{post.title}}</h3>
<i>Publié le {{ post.date }}</i>
{{post.content}}
<br />
{% endfor %}
