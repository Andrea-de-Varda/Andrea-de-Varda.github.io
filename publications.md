---
layout: default
title: Publications
permalink: /publications/
---

<h1>Publications</h1>

<div class="pub-filters">
  <span>Sorted by year (newest first)</span>
</div>

{% assign pubs = site.data.publications | sort: 'year' | reverse %}
{% for p in pubs %}
  <div class="pub-item">
    <div class="pub-head">
      <span class="pub-year">{{ p.year }}</span>
      <h2 class="pub-title">{{ p.title }}</h2>
    </div>
    <div class="pub-authors">{{ p.authors }}</div>
    <div class="pub-venue">{{ p.venue }}</div>
    <div class="pub-links">
      {% if p.doi %}<a href="https://doi.org/{{ p.doi }}">DOI</a>{% endif %}
      {% if p.url %}<a href="{{ p.url }}">Journal</a>{% endif %}
      {% if p.pdf %}<a href="{{ p.pdf }}">PDF</a>{% endif %}
      {% if p.code %}<a href="{{ p.code }}">Code</a>{% endif %}
      {% if p.preprint %}<a href="{{ p.preprint }}">Preprint</a>{% endif %}
    </div>
  </div>
{% endfor %}

<p class="pub-note">In case you want a pdf version of one of these papers, please email me!</p>
