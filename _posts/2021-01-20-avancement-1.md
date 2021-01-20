---
layout: post
title: Avancement 1
tags: [Flutter, Frontend, Backend]
color: black
author: AntoineMeresse
excerpt_separator: <!--more-->
---

Hello ! On revient vers vous pour vous montrer l'avancement de cette semaine.

<!--more-->

# Application mobile

La dernière fois, nous vous avons montrer le début de l'application, on utilisait seulement des données entrées dans le code
pour avoir un début d'affichage.

Mais cette semaine, nous avons mis en place le début de notre API. On vous montre ça tout de suite !

## Backend

La partie backend est réalisé avec Spring boot.
Nous avons pour l'instant réalisé 3 routes qui sont :

- `http://notreapi/eskaps/` : Pour récupérer les informations de tous les escape games
- `http://notreapi/users/` : Pour récupérer les informations de nos utilisateurs
- `http://notreapi/outings/` : Pour récupérer les informations des différentes sorties

Pour l'instant, nos données sont lu depuis un fichier JSON, mais ne vous inquiètez pas, la partie de base de donnée arrive bientôt :)

Voici le résultat qu'on obtient pour les escape games actuellemnt :

![liste eskaps](../../../assets/img/api_v1.png "Liste des premiers escape games")

## Frontend

### Partie technique

Flutter utilise un système de widget pour ses composants. Dans notre cas, 2 widgets utilisent les mêmes données : la carte et la liste.

Afin de séparer la partie UI & données, Flutter propose une architecture de BLoC (Business Logic Components).
Les blocs sont des composants réactifs : ils utilisent les flux de données.

Voici une image présentant les blocs :

![bloc](../../../assets/img/bloc_architecture.png "Architecture Bloc")

Mettre en place cette solution n'a pas été évident, mais le tout semble fonctionner :D

### Vidéo

Nous allons quand même vous montrer une petite vidéo de notre avancement !

<iframe width="800" height="500" src="https://youtu.be/rDSxufaPjxg" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Et oui, c'est bien les résultats que nous avons vu précédemment dans la partie API !
