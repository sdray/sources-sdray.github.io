---
# Documentation: https://wowchemy.com/docs/managing-content/

title: A critical issue in model-based inference for studying trait-based community
  assembly and a solution
subtitle: ''
summary: ''
authors:
- Cajo ter Braak
- Stéphane Dray
- Pedro Peres-Neto
tags: []
categories: []
date: '2017-01-01'
lastmod: 2022-09-27T14:50:52+02:00
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
publishDate: '2022-09-27T14:12:56.558881Z'
publication_types:
- '2'
abstract: 'Statistical testing of trait-environment association from data is a challenge
  as there is no common unit of observation: the trait is observed on species, the
  environment on sites and the mediating abundance on species-site combinations. A
  number of correlation-based methods, such as the community weighted trait means
  method (CWM), the fourth-corner correlation method and the multivariate method RLQ,
  have been proposed to estimate such trait-environment associations. In these methods,
  valid statistical testing proceeds by performing two separate resampling tests,
  one site-based and the other species-based and by assessing significance by the
  largest of the two p-values (the pmax test). Recently, regression-based methods
  using generalized linear models (GLM) have been proposed as a promising alternative
  with statistical inference via site-based resampling. We investigated the performance
  of this new approach along with approaches that mimicked the pmax test using GLM
  instead of fourth-corner. By simulation using models with additional random variation
  in the species response to the environment, the site-based resampling tests using
  GLM are shown to have severely inflated type I error, of up to 90%, when the nominal
  level is set as 5%. In addition, predictive modelling of such data using site-based
  cross-validation very often identified trait-environment interactions that had no
  predictive value. The problem that we identify is not an “omitted variable bias”
  problem as it occurs even when the additional random variation is independent of
  the observed trait and environment data. Instead, it is a problem of ignoring a
  random effect. In the same simulations, the GLM-based pmax test controlled the type
  I error in all models proposed so far in this context, but still gave slightly inflated
  error in more complex models that included both missing (but important) traits and
  missing (but important) environmental variables. For screening the importance of
  single trait-environment combinations, the fourth-corner test is shown to give almost
  the same results as the GLM-based tests in far less computing time.'
publication: '*PeerJ*'
doi: 10.7717/peerj.2885
---
