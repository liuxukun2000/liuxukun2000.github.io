---
layout: archive
comments: true
title: "Projects"
permalink: /projects/
author_profile: true
redirect_from:
  - /project
---

{% include base_path %}

{% for post in site.projects reversed %}
  {% include archive-single.html %}
{% endfor %}
