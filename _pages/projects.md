---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: false
read_more: disabled
classes: wide

#sidebar: 
#- title: "Projects"
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign projects = site.projects %}
{% endif %}

{% for post in projects %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}

{{ projects }}