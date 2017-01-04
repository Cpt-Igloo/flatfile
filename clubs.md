---
layout: default
title: Clubs de Ligue 1
---

<ul>
  {% for clubs in site.data.clubs.clubs %}
      <li>{{ clubs.key }} : {{ clubs.name}} </li>
  {% endfor %}    
</ul>
