---
title: О сайте
---

{% for image in site.static_files %}
{% if image.path contains 'images' %}
  <p>{{image.path}} - {{image.modified_time}}</p>
{% endif %}
{% endfor %}
