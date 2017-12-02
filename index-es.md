---
#
# Here you can change the text shown in the Home page before the Latest Posts section.
#
# Edit jekyll-theme-simple-blog's home layout in _layouts instead if you wanna make some changes
# See: https://jekyllrb.com/docs/themes/#overriding-theme-defaults
#
layout: home
permalink: /index.html
header:
  image: /assets/img/home-header.jpg
tagline: Cambio social y ciudadano
excerpt: >
  Somos profesoras y profesores de distintas facultades y escuelas de la Universidad de Sevilla, profesionales, estudiantes y en general personas con experiencia en la participación social preocupados por la prolongada situación de estancamiento que vive Andalucía. Nuestra tierra tiene graves carencias sociales, económicas y políticas que es necesario abordar con rigor y honestidad. Creemos que con un pie en la Universidad tenemos adquirida una responsabilidad con la sociedad, de la que formamos parte, y a la que nos debemos.
ref: home
lang: es
---
{% for post in site.posts limit:1%}
<h2><a href="{{ post.url | prepend: site.baseurl }}"> Siguiente evento</a></h2>
<img src="{{ post.poster | prepend: site.baseurl }}" alt="{{ post.title }}" title="{{ post.title }}">
{% endfor %}

<h2>¿Quienes somos?</h2>
Somos profesoras y profesores de distintas facultades y escuelas de la Universidad de Sevilla, profesionales, estudiantes y en general personas con experiencia en la participación social preocupados por la prolongada situación de estancamiento que vive Andalucía. Nuestra tierra tiene graves carencias sociales, económicas y políticas que es necesario abordar con rigor y honestidad. Creemos que con un pie en la Universidad tenemos adquirida una responsabilidad con la sociedad, de la que formamos parte, y a la que nos debemos.

Horizonte Andalucía nace como una serie de iniciativas que llevaremos a cabo para hacer participe al conjunto de la sociedad andaluza de la búsqueda de nuevas políticas que traigan desarrollo social y bienestar. Políticas que, hace tiempo, no están llegando desde nuestras instituciones.

Pensamos que en la situación política actual, auténticas soluciones solo pueden nacer de las propuestas de las numerosas organizaciones de la sociedad civil que se extienden a lo largo y ancho de Andalucía, y del conocimiento que genera la Universidad y resto del mundo academico. Por ello, invitamos a participar en el acto Horizonte Andalucía a todas las organizaciones que están trabajando en soluciones desde y para nuestra tierra.

<h2>Últimos eventos</h2>
<div>&nbsp;</div>
{% include list-category-posts.html lang=page.lang category="projects" max=3 %}
