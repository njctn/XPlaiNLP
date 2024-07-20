---
layout: archive
title: "News"
permalink: /news/
author_profile: false
read_more: disabled
url: /
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.news %}
{% endif %}

{% comment %}
{% include base_path %}
{% endcomment %}

{% for post in posts %}
    {% include archive-single.html %} 
{% endfor %}

{{ paginator }}
