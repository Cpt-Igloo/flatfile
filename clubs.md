---
title: Clubs de Ligue 1
layout: default
---

<ul>
  {% for clubs in site.data.clubs.clubs %}
      <li>{{ clubs.key }} : {{ clubs.name}} </li>
  {% endfor %}    
</ul>
