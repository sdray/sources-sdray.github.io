---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'PhylteR: Efficient Identification of Outlier Sequences in Phylogenomic Datasets'
subtitle: ''
summary: ''
authors:
- Aurore Comte
- Théo Tricou
- Eric Tannier
- Julien Joseph
- Aurélie Siberchicot
- Simon Penel
- Rémi Allio
- Frédéric Delsuc
- Stéphane Dray
- Damien M De Vienne
tags: []
categories: []
date: '2023-11-01'
lastmod: 2024-09-09T11:27:35+02:00
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
publishDate: '2024-09-09T09:27:35.156300Z'
publication_types:
- '2'
abstract: Abstract             In phylogenomics, incongruences between gene trees,
  resulting from both artifactual and biological reasons, can decrease the signal-to-noise
  ratio and complicate species tree inference. The amount of data handled today in
  classical phylogenomic analyses precludes manual error detection and removal. However,
  a simple and efficient way to automate the identification of outliers from a collection
  of gene trees is still missing. Here, we present PhylteR, a method that allows rapid
  and accurate detection of outlier sequences in phylogenomic datasets, i.e. species
  from individual gene trees that do not follow the general trend. PhylteR relies
  on DISTATIS, an extension of multidimensional scaling to 3 dimensions to compare
  multiple distance matrices at once. In PhylteR, these distance matrices extracted
  from individual gene phylogenies represent evolutionary distances between species
  according to each gene. On simulated datasets, we show that PhylteR identifies outliers
  with more sensitivity and precision than a comparable existing method. We also show
  that PhylteR is not sensitive to ILS-induced incongruences, which is a desirable
  feature. On a biological dataset of 14,463 genes for 53 species previously assembled
  for Carnivora phylogenomics, we show (i) that PhylteR identifies as outliers sequences
  that can be considered as such by other means, and (ii) that the removal of these
  sequences improves the concordance between the gene trees and the species tree.
  Thanks to the generation of numerous graphical outputs, PhylteR also allows for
  the rapid and easy visual characterization of the dataset at hand, thus aiding in
  the precise identification of errors. PhylteR is distributed as an R package on
  CRAN and as containerized versions (docker and singularity).
publication: '*Molecular Biology and Evolution*'
doi: 10.1093/molbev/msad234
links:
- name: URL
  url: https://academic.oup.com/mbe/article/doi/10.1093/molbev/msad234/7330000
---
