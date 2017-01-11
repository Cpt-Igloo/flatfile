---
title: Contact
layout: page
---

Contacts github :
<ul>
{% for partners in site.data.partners %}
  <li>
    <a href="https://github.com/{{ partners.github }}">
      {{ partners.nom }} {{ partners.prenom }} 
    </a>
  </li>
{% endfor %}
</ul>


Tel : 06 07 08 09 10
Mail : aaa@bbb.fr
