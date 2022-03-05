---
layout: default
title: "Blog"
---

{% if site.show_excerpts %}
  {% include home.html %}
{% else %}
  {% include archive.html title="Data Science" %}
  {% include archive.html title= "Finance" %}
   {% include archive.html title="Statistics" %}
{% endif %}
