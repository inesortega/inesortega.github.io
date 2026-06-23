---
layout: archive
title: "R&D Projects"
permalink: /projects/
---

<p class="page-intro">Selected participation in competitive European, national, and regional R&amp;D projects, as principal investigator, coordinator, work-package leader, technical lead, or research team member.</p>

{% assign he = site.projects | where: 'type', 'he' %}
{% assign h2020 = site.projects | where: 'type', 'h2020' %}
{% assign intl = site.projects | where: 'type', 'international' %}
{% assign international = he | concat: h2020 | concat: intl | sort: 'date' | reverse %}
{% if international.size > 0 %}
<section class="cv-section">
  <h2>International Projects</h2>
  {% for post in international %}{% include entry-project.html %}{% endfor %}
</section>
{% endif %}

{% assign national = site.projects | where: 'type', 'national' | sort: 'date' | reverse %}
{% if national.size > 0 %}
<section class="cv-section">
  <h2>National &amp; Regional Projects</h2>
  {% for post in national %}{% include entry-project.html %}{% endfor %}
</section>
{% endif %}
