---
layout: midnight
title: Code & Coffee Blagnac GitHub project page
---

## Bienvenue sur le site GitHub de Code & Coffee Blagnac !

Ce site référence les dépôts git des Kata du Code & Coffee de Blagnac.

### Organisation

L'organisation des sessions Code & Coffee de Blagnac se fait via le site Meetup de la communauté Software Craftmanship de Toulouse : [http://www.meetup.com/Software-Craftsmanship-Toulouse/](http://www.meetup.com/Software-Craftsmanship-Toulouse/). Cherchez les événements "Code and Coffee (Blagnac)".

### Code

Le code est dispo dans les différents dépots accessibles sur la page GitHub [CodeAndCoffeeBlagnac]({{ site.project-url }}).

Les derniers projets que nous avons faits sont :

{% for post in site.posts limit:5 %}

 * **[{{ post.title }}]({{ post.url }})** ({{ post.date | date_to_string }}) : [{{ post.repo-url }}]({{ post.repo-url }})

  > {{ post.excerpt }}
  [Plus d'information sur ce projet]({{ post.url }})

{% endfor %}
