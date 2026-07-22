---
layout: default
title: "Research"
permalink: /research/
---

<h1>Research</h1>

<p>
My research develops <strong>interpretable statistical learning methods</strong> for two main classes
of data: <em>natural language text</em> and <em>preference rankings</em>. The thread connecting
them is a preference for methods whose decisions can be explained and whose results can be audited.
</p>

<h2>Sentiment analysis from raw text</h2>

<p>
My doctoral and post-doctoral work has produced <strong>General Sentiment Decomposition</strong> —
a framework for mining opinions directly from unprocessed natural language, without depending on
heavy supervised pipelines. The line continues with two recent classifiers I co-designed: the
<em>Threshold-based Naïve Bayes classifier</em> (Tb-NB) and its iterative refinement (iTb-NB),
which combine competitive accuracy with the interpretability that classical Bayes models afford.
Applications have ranged from tourism reviews on Booking.com to a sentiment study of Dante's
<em>Divina Commedia</em>.
</p>

<p style="font-family: var(--font-mono); font-size: 0.8125rem; color: var(--ink-faint);">
key references: Romano, Conversano (2025, MLwA); Romano, Zammarchi, Conversano (2023, SMA);
Romano, Contu, Mola, Conversano (2023, ADAC); Romano (PhD thesis, 2021).
</p>

<h2>Preference learning and rank aggregation</h2>

<p>
A second strand of work concerns <strong>consensus ranking</strong> when many objects must be
ordered from heterogeneous judgments. With co-authors I have proposed a heuristic algorithm
scalable to large object sets, a Particle Swarm Optimization approach to preference rankings,
and most recently a distance-based aggregation method for the more general case of
<em>preference-approvals</em>.
</p>

<p style="font-family: var(--font-mono); font-size: 0.8125rem; color: var(--ink-faint);">
key references: Albano, Romano (2026, ADAC); Romano, Conversano, Siciliano, D'Ambrosio (2025, ADAC);
Romano, Siciliano (CLADAG 2023).
</p>

<h2>Semi-supervised methods on text</h2>

<p>
With Marco Ortu, Andrea Carta, Luca Frigau and others, I work on
<strong>semi-supervised clustering</strong> that exploits both topical structure and sentiment to
extract meaning from large collections of reviews and social media texts. Recent work also
investigates <em>green computing</em> trade-offs in multiclass text classification — accuracy
against computational and environmental cost.
</p>

<p style="font-family: var(--font-mono); font-size: 0.8125rem; color: var(--ink-faint);">
key references: Ortu, Romano, Carta (2024, BDR); Frigau, Romano, Ortu, Contu (2023, SMA);
Priola, Romano (2025, EJASA).
</p>

<h2>Software</h2>

<p>
The methods above are released as open-source R packages on CRAN:
<a href="https://cran.r-project.org/package=tbnb"><span class="mono">tbnb</span></a>
implements the Threshold-based Naïve Bayes classifiers (Tb-NB and iTb-NB), and
<a href="https://cran.r-project.org/package=TheOrdinals"><span class="mono">TheOrdinals</span></a>
implements the DIVA distance-based consensus algorithm for preference-approvals.
</p>

<h2>Funded projects (selected)</h2>

<ul>
  <li>
    <strong>e.INS — Ecosystem of Innovation for Next Generation Sardinia</strong>, Spoke 6
    (PNRR, NextGenerationEU; CUP F53C22000430001). Member; statistical methods for digital
    transformation and sustainable mobility.
  </li>
  <li>
    <strong>Digital Education Hub Higher Education</strong> (PNRR M4C1, Investment 3.4;
    CUP D43C23004530005). Member.
  </li>
  <li>
    <strong>General Sentiment Decomposition</strong> (MGR — Mobilità Giovani Ricercatori, 2025).
    Scientific Coordinator; Tokyo Metropolitan University, Japan.
  </li>
  <li>
    <strong>Context AdapteR Tree-based Framework</strong> (MGR, 2023). Scientific Coordinator;
    Constructor University Bremen, Germany.
  </li>
  <li>
    <strong>ISIDE — Innovation for Sea Safety</strong> (Interreg Italy–France Maritime 2014–2020).
    Member; data mining and predictive modeling on sea accidents.
  </li>
</ul>

<h2>Collaborators</h2>

<p>
Francesco Mola, Claudio Conversano, Giulia Contu, Giulia Zammarchi, Luca Frigau, Marco Ortu
(Cagliari); Antonio D'Ambrosio, Roberta Siciliano (Naples Federico II); Alessandro Albano (Palermo); Cristina Mollica (Sapienza University of Rome); Valeria Vitelli (Oslo); Adalbert F. X. Wilhelm (Bremen); Atsuho Nakayama (Tokyo Metropolitan);
Tomàs Aluja Banet (UPC Barcelona); José Luis García-Lapresta (Valladolid).
</p>
