---
layout: default
title: Research
permalink: /research/
---

# Research

## Multilingual neural language models
I am deeply fascinated my multilingual neural language models (MNLMs): I believe they are compelling scientific objects from a cognitive science / linguistics perspective because they encode knowledge of different languages (often in the hundreds) in a shared set of parameters. They allow us to ask deep questions about what's shared across languages at different levels of analysis (syntax, semantics, ...). Unlike humans, MNLMs can be probed at scale, intervened on, and inspected at the unit level without measurement noise. This makes them powerful tools for testing language-general hypotheses about representation and processing. At the same time, they help counter the English-centric bias of both NLP and cognitive science. My work uses MNLMs to ask whether a shared representational space emerges across languages and whether such spaces explain human behavior and brain responses.

<div class="research-card">
  <img src="{{ '/assets/img/research/interpretability.png' | relative_url }}" alt="Hidden units and multilingual structure">
  <div class="card-body">
    <h3>Interpretability of representations (syntax & semantics)</h3>
    <p>
      I analyze where and how MNLMs encode linguistic structure, testing whether the same latent dimensions support
      syntactic agreement and affective semantics across languages. I compare unit- and subspace-level analyses. Multiple studies point to the idea that these models represent the same linguistic phenomena in a consistent way across languages. <span class="muted">(see <a href="{{ '/publications/' | relative_url }}">publications</a>)</span>
    </p>
  </div>
</div>

<div class="research-card">
  <div class="card-body">
    <h3>Reading across languages & probabilistic information</h3>
    <p>
      I relate model-based predictability (e.g., surprisal, cloze measures) to eye-tracking and reading
      behaviour across multiple languages. I am particularly interested in scaling effects (model size) and how they relate to different stages of processing (early/late fixation measures). I am also interested in the interplay between memory limitations and predictability, and which architectural biases that better capture human RTs. <span class="muted">(see <a href="{{ '/publications/' | relative_url }}">publications</a>)</span>
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
