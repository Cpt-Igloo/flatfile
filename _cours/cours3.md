# Cours n°3

## Faire un menu dynamique dans Jekyll :

https://thinkshout.com/blog/2014/12/creating-dynamic-menus-in-jekyll/

Dans le fichier default.html localisé dans le dossier layouts :

>    <ul>
>      {% for p in site.pages %}
>        <li>
>          <a href="{{ p.url }}">{{ p.title }}</a>
>        </li>
>      {% endfor %}
>    </ul>

ou

>    <a {% if p.url == page.url %}class="active"{% endif %} href="{{ p.url }}">{{ p.title }}</a>
