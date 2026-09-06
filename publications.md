---
layout: default
title: Publications
description: "Publications by Andrea de Varda: journal articles, conference papers, and preprints on language and reasoning in humans and large language models."
permalink: /publications/
---

<h1>Publications</h1>

<p class="pub-filters">
  Sorted by date, newest first. <span class="legend-star"></span> Highlighted entries are selected papers. Click <em>Abstract</em> to expand it. See also my <a href="https://scholar.google.com/citations?user=Iwm9mC0AAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a> profile.
</p>

{% assign all = site.data.publications %}
{% assign sections = "preprint|Preprints & under review,journal|Journal articles,conference|Conference proceedings,chapter|Book chapters & encyclopedia entries" | split: "," %}
{% for s in sections %}
{% assign parts = s | split: "|" %}
{% assign key = parts[0] %}
{% assign label = parts[1] %}
<h2 id="{{ key }}">{{ label }}</h2>
{% for p in all %}
{% if p.type != key or p.reply %}{% continue %}{% endif %}
<div class="pub-item{% if p.highlight %} highlight{% endif %}"{% if p.id %} id="{{ p.id }}"{% endif %}>
  <div class="pub-head">
    <span class="pub-year">{{ p.year }}</span>
    <h3 class="pub-title"><a href="{{ p.url }}" target="_blank" rel="noopener">{{ p.title }}</a></h3>
  </div>
  <div class="pub-authors">{{ p.authors | replace: "Andrea Gregor de Varda", "<b>Andrea Gregor de Varda</b>" }}</div>
  <div class="pub-venue">{{ p.venue }}{% if p.note %} · {{ p.note }}{% endif %}</div>
  {% if p.award %}<div class="pub-note-inline">★ {{ p.award }}</div>{% endif %}
  <div class="pub-links">
    {% if p.url %}<a href="{{ p.url }}" target="_blank" rel="noopener">{% if p.type == "preprint" %}Preprint{% elsif p.type == "conference" %}Proceedings{% elsif p.type == "chapter" %}Publisher{% else %}Journal{% endif %}</a>{% endif %}
    {% if p.pdf %}<a href="{{ p.pdf }}" target="_blank" rel="noopener">PDF</a>{% endif %}
    {% if p.project %}<a href="{{ p.project }}" target="_blank" rel="noopener">Project page</a>{% endif %}
    {% for m in p.media %}<a href="{{ m.url }}" target="_blank" rel="noopener">{{ m.name }}</a>{% endfor %}
    {% if p.abstract %}
    <details class="abs">
      <summary>Abstract</summary>
      <div class="abs-body">{{ p.abstract }}</div>
    </details>
    {% endif %}
  </div>
  {% if p.exchange %}
  <div class="exchange">
    <h4>Discussion in PNAS</h4>
    <p class="lead">Three letters commented on this paper; each is paired with our reply.</p>
    <ol>
      {% for x in p.exchange %}
      <li>
        <span class="who">{{ x.date }} · Letter by {{ x.letter_authors }}:</span>
        <a href="{{ x.letter_url }}" target="_blank" rel="noopener">{{ x.letter_title }}</a>
        <span class="reply"><span class="who">↳ Our reply:</span> <a href="{{ x.reply_url }}" target="_blank" rel="noopener">{{ x.reply_title }}</a> <span class="who">({{ x.reply_venue }})</span></span>
      </li>
      {% endfor %}
    </ol>
  </div>
  {% endif %}
</div>
{% endfor %}
{% endfor %}
