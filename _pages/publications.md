---
layout: archive
title: "Publications"
permalink: /publications/
---

<p class="page-intro">You can also find my articles on my <a href="https://scholar.google.com/citations?hl=en&user=24Q2ayQAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar profile</a>.</p>

{% assign journals = site.publications | where: 'type', 'journal' | sort: 'date' | reverse %}
{% if journals.size > 0 %}
<section class="cv-section">
  <h2>Journal Articles</h2>
  {% for post in journals %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% assign chapters = site.publications | where: 'type', 'book-chapter' | sort: 'date' | reverse %}
{% if chapters.size > 0 %}
<section class="cv-section">
  <h2>Book Chapters</h2>
  {% for post in chapters %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% assign conferences = site.publications | where: 'type', 'conference' | sort: 'date' | reverse %}
{% if conferences.size > 0 %}
<section class="cv-section">
  <h2>Conference Papers</h2>
  {% for post in conferences %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% assign presentations = site.publications | where: 'type', 'presentation' | sort: 'date' | reverse %}
{% if presentations.size > 0 %}
<section class="cv-section">
  <h2>Conference Presentations</h2>
  {% for post in presentations %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% assign preprints = site.publications | where: 'type', 'preprint' | sort: 'date' | reverse %}
{% if preprints.size > 0 %}
<section class="cv-section">
  <h2>Preprints</h2>
  {% for post in preprints %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% assign theses = site.publications | where: 'type', 'phd' | sort: 'date' | reverse %}
{% if theses.size > 0 %}
<section class="cv-section">
  <h2>PhD Thesis</h2>
  {% for post in theses %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}
