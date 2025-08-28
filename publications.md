---
layout: default
title: Publications
permalink: /publications/
---

<h1>Publications</h1>

<div class="pub-filters">
  <span>Sorted by year (newest first)</span>
</div>

<h2>Journal Articles</h2>
{% assign journals = site.data.publications | where: "type", "journal" | sort: "year" | reverse %}
{% for p in journals %}
  <div class="pub-item">
    <div class="pub-head">
      <span class="pub-year">{{ p.year }}</span>
      <h2 class="pub-title">{{ p.title }}</h2>
    </div>
    <div class="pub-authors">{{ p.authors }}</div>
    <div class="pub-venue">{{ p.venue }}</div>
    <div class="pub-links">
      {% if p.url %}<a href="{{ p.url }}">Journal</a>{% endif %}
      {% if p.pdf %}<a href="{{ p.pdf }}">PDF</a>{% endif %}
    </div>
  </div>
{% endfor %}

<h2>Conference Proceedings</h2>
{% assign confs = site.data.publications | where: "type", "conference" | sort: "year" | reverse %}
{% for p in confs %}
  <div class="pub-item">
    <div class="pub-head">
      <span class="pub-year">{{ p.year }}</span>
      <h2 class="pub-title">{{ p.title }}</h2>
    </div>
    <div class="pub-authors">{{ p.authors }}</div>
    <div class="pub-venue">{{ p.venue }}</div>
    <div class="pub-links">
      {% if p.url %}<a href="{{ p.url }}">Proceedings</a>{% endif %}
      {% if p.pdf %}<a href="{{ p.pdf }}">PDF</a>{% endif %}
    </div>
  </div>
{% endfor %}
