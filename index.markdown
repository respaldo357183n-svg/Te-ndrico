---
layout: archive
author_profile: false
classes: wide
header:
  overlay_image: /imagenes/imagen-principal.jpg
  overlay_filter: 0.6
  caption: ""
  actions:
    - label: "Explorar artículos"
      url: /articulos/
    - label: "Sobre el proyecto"
      url: /sobre-el-proyecto/
excerpt: "Un espacio dedicado a la divulgación teológica a partir de la reflexión académica."
title: "Haciendo teología en el continente digital"
---

<h3 class="archive__subtitle">Artículos recientes</h3>

{% assign posts = site.posts %}
{% for post in posts %}
  {% include archive-single.html type="grid" %}
{% endfor %}
