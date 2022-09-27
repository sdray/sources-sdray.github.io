---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Testing the Mantel statistic with a spatially-constrained permutation procedure
subtitle: ''
summary: ''
authors:
- Julie Crabot
- Sylvie Clappe
- Stéphane Dray
- Thibault Datry
tags:
- distance decay relationships
- Mantel test
- Moran spectral randomization
- principal coordinates analysis
- spatial autocorrelation
- spatially constrained null model
- type I error inflation
categories: []
date: '2019-01-01'
lastmod: 2022-09-27T14:50:46+02:00
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
publishDate: '2022-09-27T13:40:06.178444Z'
publication_types:
- '2'
abstract: Mantel tests are widely used in ecology to assess the significance of the
  relationship between two distance matrices computed between pairs of samples. However,
  recent studies demonstrated that the presence of spatial autocorrelation in both
  distance matrices induced inflations of parameter estimates and type I error rates.
  These results also hold for partial Mantel test which is supposed to control for
  the spatial structures. To address the issue of spatial autocorrelation in testing
  the Mantel statistic, we developed a new procedure based on spatially constrained
  randomizations using Moran spectral randomization. A simulation study was conducted
  to assess the performance of this new procedure. Different scenarios were considered
  by manipulating the number of variables, the number of samples, the regularity of
  the sampling design and the level of spatial autocorrelation. As identified by previous
  studies, we found that Mantel statistic and its associated type I error rate are
  inflated in simple and partial Mantel tests when both distances matrices are spatially
  structured. We showed that these biases increased with the number of variables,
  decreased with the number of samples and were slightly lower for regular than irregular
  sampling. The new procedure succeeded in correcting the spurious inflations of the
  parameter estimates and type I error rates in any of the presented scenarios. Our
  results suggest that studies from several fields (e.g. genetic or community ecology)
  could have been overestimating the relationship between two distances matrices when
  both presented spatial autocorrelation. We proposed an alternative solution applicable
  in every field to correctly compute Mantel statistic with a fair type I error rate.
publication: '*Methods in Ecology and Evolution*'
doi: 10.1111/2041-210X.13141
---
