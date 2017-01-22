---
title: О сайте
---

<main class="fotorama" role="main">
  {% for image in site.static_files %}
    {% if image.path contains 'images' %}
      <img src="{{image.path}}" alt="{{image.name}}">
    {% endif %}
  {% endfor %}
</main>
