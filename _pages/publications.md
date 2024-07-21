---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
read_more: disabled
classes: wide
---

{% if paginator %}
  {% assign posts = paginator.posts | reverse %}
{% else %}
  {% assign posts = site.publications | reverse %}
{% endif %}

{% for post in posts %}
  {% include archive-single.html %}
  <p></p>
{% endfor %}
