---
# Documentation: https://wowchemy.com/docs/managing-content/

title: How to measure and test phylogenetic signal
subtitle: ''
summary: ''
authors:
- Tamara Münkemüller
- S Lavergne
- B. Bzeznik
- Stéphane Dray
- T Jombart
- Katja Schiffers
- Wilfried Thuiller
tags: []
categories: []
date: '2012-01-01'
lastmod: 2022-09-27T14:50:50+02:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
publishDate: '2022-09-27T14:12:55.094375Z'
publication_types:
- '2'
abstract: 1. Phylogenetic signal is the tendency of related species to resemble each
  other more than species drawn at random from the same tree. This pattern is of considerable
  interest in a range of ecological and evolutionary research areas, and various indices
  have been proposed for quantifying it. Unfortunately, these indices often lead to
  contrasting results, and guidelines for choosing the most appropriate index are
  lacking. 2. Here, we compare the performance of four commonly used indices using
  simulated data. Data were generated with numerical simulations of trait evolution
  along phylogenetic trees under a variety of evolutionary models. We investigated
  the sensitivity of the approaches to the size of phylogenies, the resolution of
  tree structure and the availability of branch length information, examining both
  the response of the selected indices and the power of the associated statistical
  tests. 3. We found that under a Brownian motion (BM) model of trait evolution, Abouheif's
  Cmean and Pagel's Lambda performed well and substantially better than Moran's I
  and Blomberg's K. Pagel's Lambda provided a reliable effect size measure and performed
  better for discriminating between more complex models of trait evolution, but was
  computationally more demanding than Abouheif's Cmean. Blomberg's K was most suitable
  to capture the effects of changing evolutionary rates in simulation experiments.
  4. Interestingly, sample size influenced not only the uncertainty but also the expected
  values of most indices, while polytomies and missing branch length information had
  only negligible impacts. 5. We propose guidelines for choosing among indices, depending
  on (a) their sensitivity to true underlying patterns of phylogenetic signal, (b)
  whether a test or a quantitative measure is required and (c) their sensitivities
  to different topologies of phylogenies. 6. These guidelines aim to better assess
  phylogenetic signal and distinguish it from random trait distributions. They were
  developed under the assumption of BM, and additional simulations with more complex
  trait evolution models show that they are to a certain degree generalizable. They
  are particularly useful in comparative analyses, when requiring a proxy for niche
  similarity, and in conservation studies that explore phylogenetic loss associated
  with extinction risks of specific clades.
publication: '*Methods in Ecology and Evolution*'
---
