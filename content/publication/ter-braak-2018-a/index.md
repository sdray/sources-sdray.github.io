---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Simple Parametric Tests for Trait– Environment Association
subtitle: ''
summary: ''
authors:
- Cajo J.F. ter Braak
- Pedro R. Peres-Neto
- Stéphane Dray
tags:
- '"community ecology"'
- '"community-level test"'
- '"cwm of traits"'
- '"environmental gradients"'
- '"fourth-corner"'
- '"functional traits"'
- '"modified test"'
- '"species niche centroid"'
- '"species-level test"'
- '"statistical ecology"'
- '"trait–environment relationship"'
categories: []
date: '2018-01-01'
lastmod: 2020-10-22T20:41:26+02:00
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
publishDate: '2020-10-22T18:41:25.685376Z'
publication_types:
- '2'
abstract: Question The community weighted means (CWM) approach is an easy way of analyzing
  trait-environment association by regressing (or correlating) the mean trait per
  plot against an environmental variable and assessing the statistical significance
  of the slope or the associated correlation coefficient. However, the CWM approach
  does not yield valid tests as random traits (or random indicator values) are far
  too often judged significantly related to the environmental variable, even when
  the trait and environmental variable are extrinsic to (not derived from) the community
  data. Existing solutions are the ZS-modified test (Zelený & Schaffers 2012) and
  the max (or sequential) test based on the fourth-corner correlation. Both tests
  are based on permutations which become cumbersome when many tests need to be carried
  out and many permutations are required as in methods that correct for multiple testing.
  The main goal of this paper is to compare these existing permutation-based solutions
  and to develop a quick and easy parametric test that can replace them. Methods This
  paper decomposes the fourth-corner correlation in two ways, which suggests a simple
  parametric approach consisting of assessing the significances of two linear regressions,
  one plot-level test as in the CWM approach and one species-level test, the reverse
  of the CWM approach, that regresses the environmental mean per species (i.e. the
  species niche centroid) on to the trait. The tests are combined by taking the maximum
  P-value. The type I error rates and power of this parametric max test is examined
  by simulation of one- and two-dimensional Gaussian models and log-linear models.
  Results The ZS-modified test and the fourth-corner max test are conservative in
  different scenarios, the ZS-modified test being even more conservative than fourth-corner.
  The new parametric max test is shown to control the type I error and has equal or
  even higher power than permutation tests based on fourth-corner, the ZS-modified
  test and variants thereof. A weighted version of the new test showed inflated type
  I error. Conclusion The combination of two simple regressions is a good alternative
  for the fourth-corner and the ZS-modified test. This combination is also applicable
  when multiple trait measurements are made per plot.
publication: '*Journal of Vegetation Science*'
doi: 10.1111/jvs.12666
---
