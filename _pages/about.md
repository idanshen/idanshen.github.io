---
permalink: /
title: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a fourth-year Ph.D. student in EECS at MIT advised by Professor [Pulkit Agrawal](https://people.csail.mit.edu/pulkitag/). I'm working on reinforcement learning algorithms and their applications, mainly in NLP and robotics. My research has been funded by [Qualcomm Innovation Fellowship](https://www.qualcomm.com/research/university-relations/innovation-fellowship/2024-north-america) and [MIT-Google Collaboration Grant](https://computing.mit.edu/mit-google-program-for-computing-innovation/).

<section class="news-section">
  <input id="news-recent-toggle" class="news-toggle__input" type="checkbox" checked aria-label="Show recent news only">
  <div class="news-section__header">
    <h2>News</h2>
    <div class="news-toggle" aria-label="News list filter">
      <span class="news-toggle__label">All</span>
      <label class="news-toggle__switch" for="news-recent-toggle">
        <span class="news-toggle__track"></span>
      </label>
      <span class="news-toggle__label">Recent</span>
    </div>
  </div>

  <div class="news-list">
    <div class="news__row" data-recent-news="true"><span class="news__date">[Apr 2026]</span><span class="news__text">Invited talk at IBM Research and UT Austin</span></div>
    <div class="news__row" data-recent-news="true"><span class="news__date">[Apr 2026]</span><span class="news__text">Interview at Deep Learning with Yacine <a href="https://www.youtube.com/watch?v=agitg8_0rlw">[Link]</a></span></div>
    <div class="news__row" data-recent-news="true"><span class="news__date">[Mar 2026]</span><span class="news__text">Invited talk at FAIR</span></div>
    <div class="news__row" data-recent-news="true"><span class="news__date">[Dec 2025]</span><span class="news__text"><i>RL's Razor</i> got the best paper award at the CCFM Workshop, Neurips 2025</span></div>
    <div class="news__row" data-recent-news="true"><span class="news__date">[Jul 2025]</span><span class="news__text"><i>Language Model Personalization via Reward Factorization</i> will be presented as an oral in MoFA Workshop, ICML 2025</span></div>
    <div class="news__row"><span class="news__date">[Sep 2024]</span><span class="news__text">Awarded the Qualcomm 2024 Innovation Fellowship</span></div>
    <div class="news__row"><span class="news__date">[Jun 2024]</span><span class="news__text">I'm joining Google DeepMind as a student researcher for summer 2024</span></div>
    <div class="news__row"><span class="news__date">[May 2024]</span><span class="news__text">I will give an oral presentation in ICLR 2024 R2-FM workshop on our <i>Value Augmented Sampling</i> paper</span></div>
    <div class="news__row"><span class="news__date">[Jan 2024]</span><span class="news__text"><i>Curiosity-driven Red-teaming for Large Language Models</i> got accepted to ICLR 2024</span></div>
    <div class="news__row"><span class="news__date">[Sep 2024]</span><span class="news__text">Teaching Assistant for <a href="https://pulkitag.github.io/6.884/sp20/"> Computational Sensorimotor Learning Course</a>.</span></div>
    <div class="news__row"><span class="news__date">[Sep 2023]</span><span class="news__text">Invited talk at Hyundai Research.</span></div>
    <div class="news__row"><span class="news__date">[Jun 2023]</span><span class="news__text">Invited talk at the Technion.</span></div>
    <div class="news__row"><span class="news__date">[Apr 2023]</span><span class="news__text">Our TGRL paper got accepted to ICML2023, see you in Hawaii!</span></div>
  </div>
</section>

{% include base_path %}

<section class="publications-section">
  <input id="publications-selected-toggle" class="publications-toggle__input" type="checkbox" checked aria-label="Show selected publications only">
  <div class="publications-section__header">
    <h2 id="publications">Publications</h2>
    <div class="publications-toggle" aria-label="Publication list filter">
      <span class="publications-toggle__label">All</span>
      <label class="publications-toggle__switch" for="publications-selected-toggle">
        <span class="publications-toggle__track"></span>
      </label>
      <span class="publications-toggle__label">Selected Publications</span>
    </div>
  </div>

  <div class="publications-section__list">
    {% assign publications = site.publications | sort: "publication_order" %}
    {% for post in publications %}
      {% include publication-home.html %}
    {% endfor %}
  </div>
</section>
