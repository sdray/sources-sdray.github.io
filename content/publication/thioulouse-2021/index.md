---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Overcoming the Spurious Groups Problem in Between-Group PCA
subtitle: ''
summary: ''
authors:
- Jean Thioulouse
- Sabrina Renaud
- Anne-Béatrice Dufour
- Stéphane Dray
tags: []
categories: []
date: '2021-12-01'
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
publishDate: '2022-09-27T14:12:56.940833Z'
publication_types:
- '2'
abstract: Several papers have recently raised the occurrence of some problems with
  between-group Principal Component Analysis (bgPCA). This method inflates the differences
  between the groups, and can even display completely artificial differences when
  none exist, for example when applied to random numbers tables with many variables
  (columns) and few individuals (rows). Lately, cross-validation has been proposed
  as a way to circumvent this problem. Here we present some tools and several functions
  of the ade4 package for the R statistical software to compute a bgPCA, test the
  presence of statistically significant groups, perform a cross-validation of this
  analysis and compute associated statistics. We also describe how to use these functions
  to avoid running into the spurious groups problem. Several examples, including a
  real data set and random numbers tables, are used to validate this approach in various
  experimental and numerical conditions. The integrated framework of the duality diagram,
  as implemented in ade4, allows to extend this approach to other multivariate analysis
  methods beyond principal component analysis, which could prove useful in the case
  of other types of variables. The R code and the real data table used to make the
  computations and graphs of this paper are available as supplementary material.
publication: '*Evolutionary Biology*'
doi: 10.1007/s11692-021-09550-0
links:
- name: URL
  url: https://link.springer.com/10.1007/s11692-021-09550-0
---
