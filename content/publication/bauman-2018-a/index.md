---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Optimizing the Choice of a Spatial Weighting Matrix in Eigenvector-Based Methods
subtitle: ''
summary: ''
authors:
- David Bauman
- Thomas Drouet
- Marie Josée Fortin
- Stéphane Dray
tags:
- '"community ecology"'
- '"community simulation"'
- '"connection scheme"'
- '"inference of ecological processes from spatial pat"'
- "\"moran's eigenvector maps (mem)\""
- '"multiscale spatial patterns"'
- '"optimization"'
- '"principal coordinates of neighbor matrices (pcnm)"'
- '"spatial autocorrelation"'
- '"spatial eigenvector mapping (sevm)"'
- '"spatial weighting matrix"'
- '"type i error rate inflation"'
categories: []
date: '2018-01-01'
lastmod: 2020-10-22T20:41:04+02:00
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
publishDate: '2020-10-22T18:41:04.164942Z'
publication_types:
- '2'
abstract: Abstract Eigenvector-mapping methods such as Moran's eigenvector maps (MEM)
  are derived from a spatial weighting matrix (SWM) that describes the relations among
  a set of sampled sites. The specification of the SWM is a crucial step, but the
  SWM is generally chosen arbitrarily, regardless of the sampling design characteristics.
  Here, we compare the statistical performances of different types of SWMs (distance-based
  or graph-based) in contrasted realistic simulation scenarios. Then, we present an
  optimization method and evaluate its performances compared to the arbitrary choice
  of the most-widely used distance-based SWM. Results showed that the distance-based
  SWMs generally had lower power and accuracy than other specifications, and strongly
  underestimated spatial signals. The optimization method, using a correction procedure
  for multiple tests, had a correct type I error rate, and had higher power and accuracy
  than an arbitrary choice of the SWM. Nevertheless, the power decreased when too
  many SWMs were compared, resulting in a trade-off between the gain of accuracy and
  the loss of power. We advocate that future studies should optimize the choice of
  the SWM using a small set of appropriate candidates. R functions to implement the
  optimization are available in the adespatial package and are detailed in a tutorial.
publication: '*Ecology*'
doi: 10.1002/ecy.2469
---