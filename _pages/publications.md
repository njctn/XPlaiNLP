---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: false
---
{% comment}
{% include base_path %}


{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}
{% endcomment %}
