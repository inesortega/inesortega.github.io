---
layout: cv
title: "Curriculum Vitae"
permalink: /cv/
pdf: /files/cv.pdf
redirect_from:
  - /resume
---

<p class="page-intro">My complete CV is also available in <a href="https://inesortega.github.io/files/cv.pdf">English (PDF)</a> and in <a href="https://editor.cvn.fecyt.es/editor/cvnOnline/0000-0002-8041-6860">Spanish (CVN)</a>.</p>

<section class="cv-section">
  <h2>Education</h2>

  <div class="cv-entry">
    <div class="cv-date">2020–2024</div>
    <div class="cv-content">
      <div class="title">PhD, Telecommunications &amp; Information Technology</div>
      <div class="org">Universidade de Vigo</div>
      <div class="details">Cum Laude, International Mention &amp; Industrial Doctorate distinction. Pre-doctoral research stay at Roma Sapienza (2023, 3 months).</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2017 - 2018</div>
    <div class="cv-content">
      <div class="title">MSc, Cybersecurity</div>
      <div class="org">Universidad Carlos III de Madrid</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2012 - 2017</div>
    <div class="cv-content">
      <div class="title">BSc, Computer Science</div>
      <div class="org">Universidad Carlos III de Madrid</div>
    </div>
  </div>
</section>

<section class="cv-section">
  <h2>Work Experience</h2>

  

  <div class="cv-entry">
    <div class="cv-date">2026–present</div>
    <div class="cv-content">
      <div class="title">Research Fellow, at Machine Alignment, Transparency & Security (MATS)</div>
      <div class="org">AI Security research fellowship, advised by Keri Warr (Anthropic). Working on inference verification mechanisms.</div>
    </div>
  </div>
  
  <div class="cv-entry">
    <div class="cv-date">2022-2026</div>
    <div class="cv-content">
      <div class="title">Technical Manager of Data Analytics &amp; AI</div>
      <div class="org">Security and Privacy Department, GRADIANT.</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2024 &amp; 2026</div>
    <div class="cv-content">
      <div class="title">Associate Lecturer</div>
      <div class="org">Statistics &amp; Operations Research Department, Universidade de Vigo</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2021–2022</div>
    <div class="cv-content">
      <div class="title">Senior Researcher / Engineer</div>
      <div class="org">Security and Privacy Department, GRADIANT</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2020–2021</div>
    <div class="cv-content">
      <div class="title">Researcher / Engineer</div>
      <div class="org">Security and Privacy Department, GRADIANT</div>
    </div>
  </div>

  <div class="cv-entry">
    <div class="cv-date">2018–2020</div>
    <div class="cv-content">
      <div class="title">Software Engineer</div>
      <div class="org">Microsoft Canada Development Centre — Core Data Engineering</div>
    </div>
  </div>
</section>

<section class="cv-section">
  <h2>Publications</h2>
  {% assign pubs = site.publications | sort: 'date' | reverse %}
  {% for post in pubs %}{% include entry-pub.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>R&amp;D Projects</h2>
  {% assign projs = site.projects | sort: 'date' | reverse %}
  {% for post in projs %}{% include entry-project.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>Software</h2>
  {% assign sw = site.software | sort: 'date' | reverse %}
  {% for post in sw %}{% include entry-software.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>Personal Projects</h2>
  {% assign pers = site.personal | sort: 'date' | reverse %}
  {% for post in pers %}{% include entry-personal.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>Teaching &amp; Supervision</h2>
  {% assign teach = site.teaching | sort: 'date' | reverse %}
  {% for post in teach %}{% include entry-teaching.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>Talks</h2>
  {% assign talks = site.talks | sort: 'date' | reverse %}
  {% for post in talks %}{% include entry-talk.html %}{% endfor %}
</section>

<section class="cv-section">
  <h2>Skills</h2>
  <p class="inline-list">
    <strong>Programming:</strong> Python, R, C, C++, Java<br>
    <strong>Project management:</strong> task &amp; work-package leader; funding acquisition; H2020 and Horizon Europe proposal preparation<br>
    <strong>Tools &amp; DevOps:</strong> Git, Docker, Jenkins, CI/CD methodologies, software design patterns, ELK stack, bash scripting<br>
    <strong>Data:</strong> SQL databases, data processing and management
  </p>
</section>
