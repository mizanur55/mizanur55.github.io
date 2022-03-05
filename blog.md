---
layout: default
title: "Blog"
---

{% if site.show_excerpts %}
  {% include home.html %}
{% else %}
  {% include archive.html title="Posts" %}
  {% include archive.html title="aq" %}
{% endif %}
