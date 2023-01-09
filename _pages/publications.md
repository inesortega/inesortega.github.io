---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

