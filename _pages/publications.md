---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---
You can also find my articles on my <u><a href="{{ author.googlescholar }}"> Google Scholar</a> profile.</u>


Journal Articles
======
<ul>{% for post in site.publications reversed %}
  {% if post.type == "journal" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

Book Chapters
======
<ul>{% for post in site.publications reversed %}
  {% if post.type == "book-chapter" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>

Conference Articles
======
<ul>{% for post in site.publications reversed %}
  {% if post.type == "conference" %}
    {% include archive-single-cv.html %}
  {% endif %}
{% endfor %}</ul>
