---
layout: default
title: Research
permalink: /research/
---

# Research

## Multilingual language models
Multilingual neural language models (MNLMs) are compelling scientific objects because they provide a single parametrized system that processes many languages, allowing controlled comparisons within one architecture. Unlike human studies, MNLMs can be probed at scale, intervened on, and inspected at the unit level without measurement noise. This makes them powerful tools for testing language-general hypotheses about representation and processing. At the same time, they help counter the English-centric bias of both NLP and cognitive science by enabling analyses across diverse typologies. My work uses MNLMs to ask whether a shared representational space emerges across languages and whether such spaces explain human behavior and brain responses.

<div class="research-card">
  <img src="{{ '/assets/img/research/interpretability.png' | relative_url }}" alt="Hidden units and multilingual structure">
  <div class="card-body">
    <h3>Interpretability of representations (syntax & semantics)</h3>
    <p>
      I analyze where and how MNLMs encode linguistic structure, testing whether the same latent dimensions support
      syntactic agreement and affective semantics across languages. I compare unit- and subspace-level signals and
      identify layers that concentrate cross-lingual structure. <span class="muted">(see <a href="{{ '/publications/' | relative_url }}">publications</a>)</span>
    </p>
  </div>
</div>

<div class="research-card">
  <div class="card-body">
    <h3>Reading across languages & probabilistic information</h3>
    <p>
      I relate model-based predictability (e.g., surprisal, cloze-aligned measures) to eye-tracking and reading
      behaviour across multiple languages, testing scaling effects (model size vs. early/late measures) and architectural
      biases that better capture human RTs. <span class="muted">(see <a href="{{ '/publications/' | relative_url }}">publications</a>)</span>
    </p>
  </div>
</div>


<div class="research-card">
  <img src="{{ '/assets/img/research/brain.png' | relative_url }}" alt="Brain responses to language across languages">
  <div class="card-body">
    <h3>Brain–model alignment across languages</h3>
    <p>
      I train encoding models to predict fMRI responses to language from MNLM embeddings and test zero-shot transfer
      across languages and families. Results point to language-general principles in neural responses to linguistic
      input. <span class="muted">(see <a href="{{ '/publications/' | relative_url }}">publications</a>)</span>
    </p>
  </div>
</div>

<p class="pub-note">
For full citations and links to journals and PDFs, see the <a href="{{ '/publications/' | relative_url }}">Publications</a> page.
</p>
