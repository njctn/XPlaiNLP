---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
read_more: disabled
---

{% if paginator %}
  {% assign posts = paginator.posts %}
{% else %}
  {% assign posts = site.publications %}
{% endif %}

{% comment %}
{% assign entries_layout = page.entries_layout | default: 'list' %}
<div class="entries-{{ entries_layout }}">
  {% for post in posts %}
    {% include archive-single.html type=entries_layout %}
  {% endfor %}
</div>
{% endcomment %}

{% include base_path %}

{% for post in posts %}
  {% include archive-single.html %}
{% endfor %}

