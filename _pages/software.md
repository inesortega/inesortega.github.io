---
layout: archive
title: "Software"
permalink: /software/
---

<p class="page-intro">Open-source scientific software for interpretable machine learning, privacy, and data anonymisation.</p>

<section class="cv-section">
  {% assign sw = site.software | sort: 'date' | reverse %}
  {% for post in sw %}{% include entry-software.html %}{% endfor %}
</section>
