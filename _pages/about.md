---
layout: about
title: Home
permalink: /
subtitle: Language Science & Artificial Intelligence · 语言科学智能
description: LaSAI is a research lab at Shanghai Jiao Tong University working at the intersection of language science and artificial intelligence.

profile:
  align: right
  image: lasai-logo.png
  image_circular: false
  address:

news: false
selected_papers: false

groups: [team]
team:
  title: Team
  people:
    - name: Ercong Nie · 聂耳聪
      description: Founder and Head · Tenure-track Assistant Professor, School of Foreign Languages, SJTU
      website: https://ercong21.github.io/
      picture: ercong-nie.jpg
    - name: This could be you!
      description: We welcome motivated students interested in multilingual AI, interpretability, language science, and human-centered NLP.
      website: /contact/
      placeholder: true
---

<div class="home-intro">
  <p class="lead">
    Welcome to <strong>LaSAI</strong> — the <strong>Language Science & Artificial Intelligence</strong>
    research lab at the <a href="https://sfl.sjtu.edu.cn/">School of Foreign Languages</a>,
    <a href="https://en.sjtu.edu.cn/">Shanghai Jiao Tong University</a>.
  </p>

  <p>
    Directed by Dr. Ercong Nie (聂耳聪) <a href="https://ercong21.github.io/">[Page]</a>, LaSAI studies
    language as both an object of artificial intelligence and a window into intelligence itself.
    We connect natural language processing, large language models, linguistics, cognition, and the
    digital humanities to build AI that is <strong>multilingual, interpretable, efficient, and human-centered</strong>.
  </p>

  <p class="bilingual-mission">
    <span>Using language science to better connect, understand, and build AI.</span>
    <span>Using AI to advance language science.</span>
    <small>以语言科学为理解智能的入口和连接智能的媒介，以人工智能拓展语言科学。</small>
  </p>

  <div class="topic-chips" aria-label="LaSAI research topics">
    <span>Multilingual AI</span>
    <span>LLM Interpretability</span>
    <span>Language & Cognition</span>
    <span>AI for Humanities</span>
  </div>
</div>

<section class="home-section" aria-labelledby="news-heading">
  <h2 class="section-heading" id="news-heading">News</h2>
  <ol class="news-list">
    <li>
      <time datetime="2026-08">August 2026</time>
      <div>
        Two papers were accepted to <a href="https://2026.emnlp.org/">EMNLP 2026</a>
        (one Main Conference paper and one Findings paper), on long-horizon video reasoning and
        mechanistic interpretability of language abilities in large language models.
        <a href="https://arxiv.org/abs/2605.17065">Main paper</a> ·
        <a href="https://www.preprints.org/manuscript/202607.1441">Findings paper</a>
      </div>
    </li>
    <li>
      <time datetime="2026-07">July 2026</time>
      <div>
        We co-organized <span lang="zh">“大语言模型与数字人文的方法和应用暨上海交通大学首届数字人文暑期高端研讨会”</span>.
        Ercong delivered the keynote <em>What Can Linguistics Bring to Large Language Models?</em>
        <a href="https://sfl.sjtu.edu.cn/post/6774">News</a> ·
        <a href="{{ '/assets/pdf/SJTU-DH2026.pdf' | relative_url }}">Slides</a>
      </div>
    </li>
    <li>
      <time datetime="2026-07">July 2026</time>
      <div>
        Our work on cross-lingual NLP for historical-language treebank construction was published in
        <em>Digital Scholarship in the Humanities</em>.
        <a href="https://doi.org/10.1093/llc/fqag104">Paper</a>
      </div>
    </li>
    <li>
      <time datetime="2026-06">June 2026</time>
      <div>
        Ercong gave an invited talk on cross-lingual failures in large language models at
        <a href="https://sites.google.com/view/jingyuan-sun/home">Jingyuan Sun's group</a>, University of Manchester.
      </div>
    </li>
    <li>
      <time datetime="2026-06">June 2026</time>
      <div>
        Ercong chaired the “Language Science and LLMs” session at the
        <a href="https://mp.weixin.qq.com/s/Vx1bKvHS2kE1wh_a156-hQ">3rd Language Science and Intelligence Forum</a>.
      </div>
    </li>
    <li>
      <time datetime="2026-06">June 2026</time>
      <div>
        LaSAI began a new chapter as Ercong joined the School of Foreign Languages at SJTU as a
        tenure-track assistant professor.
      </div>
    </li>
  </ol>
</section>

<section class="home-section team-section" aria-labelledby="team-heading">
  {%- for group in page.groups -%}
    <h2 class="section-heading" id="team-heading">{{ page[group].title }}</h2>
    <div class="team-grid">
      {%- for person in page[group].people -%}
        <article class="team-card">
          {% if person.placeholder -%}
            <div class="avatar-placeholder" aria-hidden="true">?</div>
          {%- elsif person.picture -%}
            <img class="team-avatar" src="{{ '/assets/img/' | append: person.picture | relative_url }}" alt="Portrait of {{ person.name }}">
          {%- endif %}
          <div class="team-card-body">
            <h3>
              {% if person.website -%}
                <a href="{{ person.website }}">{{ person.name }}</a>
              {%- else -%}
                {{ person.name }}
              {%- endif %}
            </h3>
            <p>{{ person.description }}</p>
          </div>
        </article>
      {%- endfor -%}
    </div>
  {%- endfor -%}
</section>

<aside class="join-callout">
  <div>
    <span class="eyebrow">Build LaSAI with us</span>
    <h2>Curious about language and intelligence?</h2>
    <p>Students from language, computer science, cognitive science, and neighboring fields are welcome.</p>
  </div>
  <a class="brand-button" href="{{ '/contact/' | relative_url }}">Get in touch</a>
</aside>
