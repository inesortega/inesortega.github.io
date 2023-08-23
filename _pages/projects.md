---
layout: archive
title: "R&D Projects"
permalink: /projects/
author_profile: true
---

## International Projects

<ul>{% for post in site.projects reversed %}
  {% if post.type == "he" %}
    {% include archive-single-project-summary.html %}
  {% elsif post.type == "h2020" %}
    {% include archive-single-project-summary.html %}
  {% endif %}
{% endfor %}</ul>

## National & Regional projects

<ul>{% for post in site.projects reversed %}
  {% if post.type == "national" %}
    {% include archive-single-project-summary.html %}
  {% endif %}
{% endfor %}</ul>