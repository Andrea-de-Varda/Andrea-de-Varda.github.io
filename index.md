---
layout: default
title: Home
permalink: /
---

<div class="hero">
  <img src="{{ '/assets/img/profile.jpg' | relative_url }}" alt="Portrait of Andrea de Varda" class="avatar">
  <div>
    <h1 class="name">Andrea de Varda</h1>
    <p class="tagline">Postdoctoral fellow, Department of Brain and Cognitive Sciences &amp; McGovern Institute for Brain Research, MIT — 📧 Email: <span class="mono">devar_ag ✶ mit ✹ edu</span></p>
    <p class="tagline">K. Lisa Yang ICoN Fellow · <a href="https://evlab.mit.edu/" target="_blank" rel="noopener">Ev Fedorenko's Language Lab</a> &amp; <a href="http://cpl.mit.edu/" target="_blank" rel="noopener">Computational Psycholinguistics Lab </a> </p>
    <div class="hero-links">
      <a href="https://scholar.google.com/citations?user=Iwm9mC0AAAAJ&hl=en" target="_blank" rel="noopener">Google Scholar</a>
      <a href="https://github.com/Andrea-de-Varda" target="_blank" rel="noopener">GitHub</a>
      <a href="https://bsky.app/profile/andreadevarda.bsky.social" target="_blank" rel="noopener">Bluesky</a>
      <a href="https://x.com/devarda_a" target="_blank" rel="noopener">X</a>
    </div>
  </div>
</div>

<section>
  <h2>About</h2>
  <p>
    I am a postdoctoral fellow at MIT, working with <a href="https://evlab.mit.edu/" target="_blank" rel="noopener">Evelina Fedorenko</a> and <a href="http://cpl.mit.edu/" target="_blank" rel="noopener">Roger Levy</a>. I study language processing, and increasingly higher-level cognition more broadly, in humans and large language models. Some broad questions I am interested in are: what are the defining features of language as a cognitive system—properties that hold across diverse languages, and between artificial and biological language systems? What makes some reasoning domains and problems hard? How is higher-level cognition organized in minds and models, and are there any privileged features that tend to emerge across systems?
    My work combines computational modeling with behavioral experiments and brain imaging, and I use language models both as tools for cognitive science and as scientific objects in their own right.
  </p>
  <p>
    I received my Ph.D. from the University of Milano-Bicocca, where I worked with <a href="https://www.marcomarelli.net/" target="_blank" rel="noopener">Marco Marelli</a> on multilingual neural language models and their relevance for cognitive science. Before that, I did a M.Sc. in Cognitive Science at the University of Trento (CIMeC).
  </p>
  <ul class="interests" aria-label="Research interests">
    <li>Language and thought in humans and LLMs</li>
    <li>Language in the brain</li>
    <li>Multilingual models</li>
    <li>Interpretability</li>
    <li>Psycholinguistics</li>
    <li>Iconicity &amp; non-arbitrariness</li>
  </ul>
</section>

<section class="sel-wrap">
  <div class="sel-head">
    <h2>Selected papers</h2>
    <div class="sel-nav">
      <button class="sel-btn" data-dir="-1" aria-label="Previous papers">&#8592;</button>
      <button class="sel-btn" data-dir="1" aria-label="Next papers">&#8594;</button>
    </div>
  </div>
  <div class="sel-track" id="sel-track">
    {% assign sel = site.data.publications | where: "highlight", true %}
    {% for p in sel %}
    <a class="sel-card" href="{{ p.url }}" target="_blank" rel="noopener">
      <span class="sel-title">{{ p.title }}</span>
      <span class="sel-body">
        {% if p.thumb %}<img src="{{ p.thumb | relative_url }}" alt="" loading="lazy">{% endif %}
        <span class="sel-meta">
          <span class="sel-authors">{{ p.authors | replace: "Andrea Gregor de Varda", "<b>A. G. de Varda</b>" }}</span>
          <span class="sel-venue">{{ p.venue | split: "," | first }}{% if p.year %}, {{ p.year }}{% endif %}</span>
        </span>
      </span>
    </a>
    {% endfor %}
  </div>
  <p class="pub-note sel-note">Full list on the <a href="{{ '/publications/' | relative_url }}">Publications</a> page.</p>
</section>
<script>
(function(){var t=document.getElementById('sel-track');if(!t)return;document.querySelectorAll('.sel-btn').forEach(function(b){b.addEventListener('click',function(){var c=t.querySelector('.sel-card');var w=c?c.getBoundingClientRect().width+16:300;t.scrollBy({left:w*parseInt(b.dataset.dir,10),behavior:'smooth'});});});})();
</script>

<section>
  <h2>News</h2>
  <ul class="news">
    <li><time>Sep 2026</time><span>Visiting <a href="https://climblab.org/" target="_blank" rel="noopener">Cory Shain's CLiMB lab</a> at Stanford (September–October 2026).</span></li>
    <li><time>Aug 2026</time><span>Two new preprints: <a href="https://arxiv.org/abs/2608.13567" target="_blank" rel="noopener">Modular cognitive architecture emerges in large language models</a> (led by Pengrui Han, with Jacob Andreas and Ev Fedorenko) and <a href="https://www.biorxiv.org/content/10.64898/2026.08.21.746238v1" target="_blank" rel="noopener">Behavioral and brain responses to language reflect different levels of linguistic representation</a> (with Yevgeni Berzak, Ev Fedorenko, and Roger Levy).</span></li>
    <li><time>Jul 2026</time><span>Invited talks at the CogSci 2026 workshop <em>Laying the foundations for foundation models of cognition</em> (Rio de Janeiro), the Deep Linguistic Modeling colloquium at Heinrich-Heine-Universität Düsseldorf, and the MilaNLP lab at Bocconi University.</span></li>
    <li><time>Jul 2026</time><span>Daria Kryvosheieva's paper <a href="https://aclanthology.org/2026.acl-long.7/" target="_blank" rel="noopener">Different types of syntactic agreement recruit the same units within large language models</a> is out at ACL 2026.</span></li>
    <li><time>Jun 2026</time><span>I was awarded a <strong>Gemini Academic Program Award</strong> from Google DeepMind.</span></li>
    <li><time>Jun 2026</time><span>I gave a keynote at the Multilingual Minds &amp; Machines Meeting (Radboud University, Nijmegen); talks at the University of Amsterdam and the University of Milano-Bicocca.</span></li>
    <li><time>May 2026</time><span>My dissertation received the <strong>Glushko Dissertation Prize</strong> from the Cognitive Science Society.</span></li>
    <li><time>May 2026</time><span>Large-scale collaboration on <a href="https://www.pnas.org/doi/10.1073/pnas.2524747123" target="_blank" rel="noopener">AI-assisted vs. human-only teams in assessing research reproducibility</a> (Brodeur et al.) published in PNAS.</span></li>
  </ul>
  <details class="news-more">
    <summary>Older news</summary>
    <ul class="news">
      <li><time>Jan–Apr 2026</time><span>Three letters on <em>The cost of thinking</em> and our replies appeared in PNAS. See the <a href="{{ '/publications/#cost-of-thinking' | relative_url }}">exchange</a> on the publications page.</span></li>
      <li><time>Mar 2026</time><span>I gave a talk on language and reasoning in models and humans at the Language and Cognition series, Harvard.</span></li>
      <li><time>Feb 2026</time><span>Patrick J. McGovern Travel &amp; Technology Award (MIT); talk at INRIA Lille.</span></li>
      <li><time>Jan 2026</time><span>Talk on compositionality and reasoning at the Workshop on Neural-Symbolic Reasoning, University of Warsaw.</span></li>
      <li><time>Dec 2025</time><span><a href="https://journals.plos.org/plosone/article?id=10.1371/journal.pone.0337947" target="_blank" rel="noopener">IconicITA</a>, iconicity ratings for the Italian affective lexicon, published in PLOS One.</span></li>
      <li><time>Nov 2025</time><span><a href="https://www.pnas.org/doi/10.1073/pnas.2520077122" target="_blank" rel="noopener">The cost of thinking is similar between large reasoning models and humans</a> published in PNAS. Covered by <a href="https://news.mit.edu/2025/cost-of-thinking-1119" target="_blank" rel="noopener">MIT News</a>.</span></li>
      <li><time>Sep 2025</time><span>Journal Club piece in <a href="https://www.nature.com/articles/s44159-025-00490-6" target="_blank" rel="noopener">Nature Reviews Psychology</a> on learning meaning from latent patterns in language use.</span></li>
      <li><time>Jun 2025</time><span>Correspondence in <a href="https://www.nature.com/articles/s41562-025-02224-3" target="_blank" rel="noopener">Nature Human Behaviour</a> on the high variability of LLMs' analogical reasoning.</span></li>
      <li><time>Mar 2025</time><span>Started as a postdoctoral fellow at MIT, working with Ev Fedorenko and Roger Levy.</span></li>
      <li><time>Feb 2025</time><span>Defended my Ph.D. at the University of Milano-Bicocca.</span></li>
      <li><time>Nov 2024</time><span>I was awarded the K. Lisa Yang Integrative Computational Neuroscience (ICoN) Fellowship at MIT.</span></li>
    </ul>
  </details>
</section>

