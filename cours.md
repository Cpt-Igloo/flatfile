---
title: Cours
layout: page
---

{% for cours in site.cours %}
  <div class="cours">
    {{ cours.content }}
  </div>
{% endfor %}
