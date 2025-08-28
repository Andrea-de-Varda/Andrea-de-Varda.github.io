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

## Non-arbitrariness and iconicity

Language is not fully arbitrary. My work examines systematic sound–meaning links using computational tools, behavioral data, and cross-lingual evaluation.

<div class="research-card">
  <img src="{{ '/assets/img/research/multilingual.jpg' | relative_url }}" alt="Cross-lingual transfer of phonosemantic patterns">
  <div class="card-body">
    <h3>Cross-lingual phonosemantic correspondences</h3>
    <p>
      We train sequence models to map phonetic representations to sensory, semantic, and word-class targets across typologically distant languages, and test zero-shot transfer (so that the models are trained to map sound onto meaning representations in, say, English, and then tested in Tamil). Successful transfer indicates language-invariant cues linking form to meaning and syntactic class.
      <span class="muted">(see <em>A Cross-Modal and Cross-lingual Study of Iconicity in Language</em>, Cognitive Science)</span>
    </p>
  </div>
</div>

<div class="research-card">
  <img src="{{ '/assets/img/research/pseudowords.png' | relative_url }}" alt="Interpretable meanings for pseudowords">
  <div class="card-body">
    <h3>Meaning beyond lexicality (pseudowords)</h3>
    <p>
      Using exploratory–confirmatory designs, we test whether people (and language models) can ascribe  declarative meanings to novel word forms. Human definitions and model outputs show systematic form-to-meaning mappings, supporting flexible generalization beyond the existing lexicon.
      <span class="muted">(see <em>Meaning Beyond Lexicality: Capturing Pseudoword Definitions with Language Models</em>, Computational Linguistics, Open Access)</span>
    </p>
  </div>
</div>

<div class="research-card">
  <img src="{{ '/assets/img/research/PBR.png' | relative_url }}" alt="Auditory resemblance between words and sounds">
  <div class="card-body">
    <h3>Auditory iconicity at scale</h3>
    <p>
      We embed natural sounds and spoken words into a shared auditory space (STFT, CNNs for sound and speech classification) to quantify direct resemblance between word sounds (e.g., the sound of the word "frog") and natural sounds (e.g., the sound of a frog croaking). Auditory imitation is widespread across the English auditory vocabulary, and aligns with human iconicity judgments.
      <span class="muted">(see <em>Cracking Arbitrariness: A Data-driven Study of Auditory Iconicity in Spoken English</em>, Psychonomic Bulletin &amp; Review)</span>
    </p>
  </div>
</div>


<p class="pub-note">
For full citations and links to journals and PDFs, see the <a href="{{ '/publications/' | relative_url }}">Publications</a> page.
</p>
