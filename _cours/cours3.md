# Cours n°3

## Faire un menu dynamique dans Jekyll :

https://thinkshout.com/blog/2014/12/creating-dynamic-menus-in-jekyll/

Dans le fichier default.html localisé dans le dossier layouts :

{% raw %}
    <ul>
      {% for p in site.pages %}
        <li>
          <a href="{{ p.url }}">{{ p.title }}</a>
        </li>
      {% endfor %}
    </ul>
{% endraw %}


ou

    <a {% if p.url == page.url %}class="active"{% endif %} href="{{ p.url }}">{{ p.title }}</a>


## Lister les contenus d'un post sur une page :
Les postes de blogs doivent être créés dans le dossier posts sour le format "YYYY-MM-DD-nom-de-l'article"
>{% for post in site.posts %}

><h3>{{post.title}}</h3>

><i>Publié le {{ post.date }}</i>

>{{post.content}}

>{% endfor %}
