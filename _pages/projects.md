---
layout: archive
title: "My Projectsvv"
permalink: /projects/
author_profile: true
redirect_from:
  - /project
---

{% include base_path %}

{% for post in site.teaching reversed %}
  {% include archive-single.html %}
{% endfor %}
