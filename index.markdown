---
layout: home
author_profile: false
classes: wide
---

{% assign posts = site.posts %}
{% for post in posts %}
  {% include archive-single.html type="grid" %}
{% endfor %}
