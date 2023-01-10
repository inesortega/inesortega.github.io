---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
You can also find my articles on my <a href="https://scholar.google.com/citations?hl=en&user=pz0SDFAAAAAJ&view_op=list_works&sortby=pubdate"> Google Scholar</a> profile.

### Journal Articles

<ul>{% for post in site.publications reversed %}
  {% if post.type == "journal" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

### Book Chapters

<ul>{% for post in site.publications reversed %}
  {% if post.type == "book-chapter" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

### Conference Articles

<ul>{% for post in site.publications reversed %}
  {% if post.type == "conference" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>
