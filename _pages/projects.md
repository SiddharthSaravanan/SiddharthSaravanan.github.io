---
layout: archive
title: "My Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /project
---

{% include base_path %}

{% for post in site.teaching reversed %}
  {% include category-list.html %}
{% endfor %}
