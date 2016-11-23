# COURS N°2

##Installer Jekyll

Jekyll est un générateur de site statique utilisant le langage Ruby.

###Installer Jekyll sur ubuntu :

Il faut d'abord installer Ruby avec la commande suivante :
>sudo apt-get install ruby ruby-dev make gcc nodejs

Commande pour installer Jekyll :
>sudo gem install jekyll --no-rdoc --no-ri

Vérifier que Jekyll est bien installé :
>jekyll -v

Lancer Jekyll (ancienne méthode, fait un watch par défaut) :
>jekyll serve

Lancer Jekyll et créer un site :
>jekyll build


Mettre Jekyll à jour :
>sudo gem update jekyll --no-rdoc --no-ri

Installer des fonctionnalités dans Jekyll :
>sudo gem install github-pages --no-rdoc --no-ri

##Fonctionnement de Jekyll

Fichiers avec un underscore : Ne sont pas générés dans le site

Créer des fichiers includes :
Il s'agit de créer des fichiers contenant par exemple le header et le footer qui seront appelés à chaque fois
sur la page web.
On créé un dossier *_includes* dans lequel on mettra le head, le footer, et le header en html qui seront
appelés sur la page principale.
>{% include head.html %}

##Répertoires de flatfiles :

-**_includes** : Regroupe les fichiers à inclure dans chaque page html, généralement le head, le header le footer

-**_layouts** (gabarit en français) : Regroupe des templates de pages (nommé default.html)

-**_site** : A chaque lancement du serveur reprend les pages web modifiés

## A mettre sur les fichiers md de pages :

  ---
  layout: default
  title: Accueil
  ---

## Appeler un titre
>{{site.title}} : {{page.title}}

## Appeler un élément "include"
>{% include head.html %}

head.html se trouvant dans le dossier includes

## Appeler un layout
>---
>layout: defaut
>---

Le layout est un modèle de page se trouvant dans le dossier du même nom

## Lancer le serveur Jekyll
Taper dans le terminal >jekyll serve
