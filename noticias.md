---
title: "Noticias"
layout: archive
permalink: /noticias/
author_profile: false
classes: wide
---

{% assign noticias = site.posts | where_exp: "post", "post.categories contains 'Noticias'" %}
{% for post in noticias %}
  {% include archive-single.html type="list" %}
{% endfor %}
