---
layout: archive
title: "News"
permalink: /news/
author_profile: false
read_more: disabled
classes: wide
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.news %}
{% endif %}

{% for post in posts %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
