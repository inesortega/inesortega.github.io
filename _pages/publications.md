---
layout: archive
title: "Publications"
permalink: /publications/
---

<p class="page-intro">You can also find my articles on my <a href="https://scholar.google.com/citations?hl=en&user=24Q2ayQAAAAJ&view_op=list_works&sortby=pubdate">Google Scholar profile</a>.</p>

{% assign journals = site.publications | where: 'type', 'journal' | sort: 'date' | reverse %}
{% assign chapters = site.publications | where: 'type', 'book-chapter' | sort: 'date' | reverse %}
{% assign conferences = site.publications | where: 'type', 'conference' | sort: 'date' | reverse %}
{% assign presentations = site.publications | where: 'type', 'presentation' | sort: 'date' | reverse %}
{% assign preprints = site.publications | where: 'type', 'preprint' | sort: 'date' | reverse %}
{% assign theses = site.publications | where: 'type', 'phd' | sort: 'date' | reverse %}

<div class="pub-filters">
  <button type="button" class="pub-filter is-active" data-filter="all">All</button>
  {% if journals.size > 0 %}<button type="button" class="pub-filter" data-filter="journal">Journals</button>{% endif %}
  {% if conferences.size > 0 %}<button type="button" class="pub-filter" data-filter="conference">Conference</button>{% endif %}
  {% if presentations.size > 0 %}<button type="button" class="pub-filter" data-filter="presentation">Presentations</button>{% endif %}
  {% if chapters.size > 0 %}<button type="button" class="pub-filter" data-filter="book-chapter">Book Chapters</button>{% endif %}
  {% if preprints.size > 0 %}<button type="button" class="pub-filter" data-filter="preprint">Preprints</button>{% endif %}
  {% if theses.size > 0 %}<button type="button" class="pub-filter" data-filter="phd">Thesis</button>{% endif %}
</div>

{% if journals.size > 0 %}
<section class="cv-section" data-pubtype="journal">
  <h2>Journal Articles</h2>
  {% for post in journals %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% if conferences.size > 0 %}
<section class="cv-section" data-pubtype="conference">
  <h2>Conference Papers</h2>
  {% for post in conferences %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% if presentations.size > 0 %}
<section class="cv-section" data-pubtype="presentation">
  <h2>Conference Presentations</h2>
  {% for post in presentations %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% if chapters.size > 0 %}
<section class="cv-section" data-pubtype="book-chapter">
  <h2>Book Chapters</h2>
  {% for post in chapters %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% if preprints.size > 0 %}
<section class="cv-section" data-pubtype="preprint">
  <h2>Preprints</h2>
  {% for post in preprints %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

{% if theses.size > 0 %}
<section class="cv-section" data-pubtype="phd">
  <h2>PhD Thesis</h2>
  {% for post in theses %}{% include entry-pub.html %}{% endfor %}
</section>
{% endif %}

<script>
  (function () {
    var filters = document.querySelectorAll('.pub-filter');
    var sections = document.querySelectorAll('[data-pubtype]');
    filters.forEach(function (btn) {
      btn.addEventListener('click', function () {
        var f = btn.getAttribute('data-filter');
        filters.forEach(function (b) { b.classList.toggle('is-active', b === btn); });
        sections.forEach(function (sec) {
          sec.hidden = !(f === 'all' || sec.getAttribute('data-pubtype') === f);
        });
      });
    });
  })();
</script>
