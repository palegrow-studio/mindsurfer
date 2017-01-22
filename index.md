---
title: О сайте
---

<main
  class="fotorama"
  role="main"
  data-width="100%"
  data-height="100%"
	data-nav="thumbs"
  data-transition="crossfade"
  data-hash="true"
  data-loop="true"
  data-keyboard="true"
  data-click="true"
  data-swipe="true">
  {% for image in site.static_files %}
    {% if image.path contains 'images' %}
      <a href="{{image.path}}" title="{{image.name}}"></a>
    {% endif %}
  {% endfor %}
</main>
