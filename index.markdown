---
layout: archive
author_profile: false
classes: wide
header:
  overlay_image: /imagenes/imagen-principal.jpg
  overlay_filter: 0.6
  actions:
    - label: "Explorar artículos"
      url: /articulos/
    - label: "Sobre el Proyecto"
      url: /sobre-el-proyecto/
excerpt: "Un espacio dedicado a la divulgación teológica a partir de la reflexión académica."
title: "Haciendo teología en el continente digital"
---

<div style="background:#f5f5f0;border:1px solid #e5e5e0;padding:1.5rem;margin-bottom:3rem;display:flex;gap:1.5rem;align-items:center;flex-wrap:nowrap;">
  <img src="/imagenes/libro-jesus-aproximacion-historica.jpg" alt="Jesús: Aproximación histórica" style="width:80px;box-shadow:0 4px 12px rgba(0,0,0,0.2);flex-shrink:0;">
  <div style="flex:1;">
    <div style="font-size:0.7rem;letter-spacing:0.1em;text-transform:uppercase;background:#f5c842;color:#1a1a1a;display:inline-block;padding:0.15rem 0.5rem;margin-bottom:0.5rem;">Club de Lectura</div>
    <h3 style="font-family:Georgia,serif;font-weight:normal;margin:0 0 0.2rem 0;font-size:1.1rem;">Jesús: Aproximación histórica</h3>
    <p style="color:#6b6b6b;margin:0 0 0.5rem 0;font-size:0.85rem;">José Antonio Pagola</p>
    <p style="margin:0 0 1rem 0;font-size:0.9rem;">Estamos leyendo juntos una de las obras más rigurosas sobre el Jesús histórico.</p>
    <a href="/club-de-lectura/" style="display:inline-block;padding:0.5rem 1.2rem;background:#1a1a1a;color:#fff!important;text-decoration:none;font-size:0.85rem;border-radius:4px;">Ver más</a>
  </div>
</div>

<h3 class="archive__subtitle">Artículos recientes</h3>

{% assign posts = site.posts %}
{% for post in posts %}
  {% include archive-single.html type="grid" %}
{% endfor %}
