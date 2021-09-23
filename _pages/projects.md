---
layout: archive
title: "My Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /project
---

{% include base_path %}

{% for post in site.portfolio reversed %}
  {% include archive-single-talk.html %}
{% endfor %}
