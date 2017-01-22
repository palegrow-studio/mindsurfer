---
title: О сайте
---

<main
  class="fotorama"
  role="main"
  data-width="100%"
  data-height="100%"
  data-fit="cover"
	data-nav="none"
>
  {% for image in site.static_files %}
    {% if image.path contains 'images' %}
      <img src="{{image.path}}" alt="{{image.name}}">
    {% endif %}
  {% endfor %}
</main>
