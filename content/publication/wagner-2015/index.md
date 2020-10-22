---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Generating Spatially Constrained Null Models for Irregularly Spaced Data Using
  Moran Spectral Randomization Methods
subtitle: ''
summary: ''
authors:
- Helene H. Wagner
- Stéphane Dray
tags: []
categories: []
date: '2015-01-01'
lastmod: 2020-10-22T20:41:28+02:00
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
publishDate: '2020-10-22T18:41:28.568846Z'
publication_types:
- '2'
abstract: "Spatial autocorrelation jeopardizes the validity of statistical inference,\
  \ for example correlation and regression analysis. Restricted randomization methods\
  \ can account for the effect of spatial autocorrelation in the observed data by\
  \ building it into an empirical null model for hypothesis testing. This can be achieved,\
  \ for example, based on conditional simulation, which fits a highly parameterized\
  \ geostatistical model to the observed spatial structure, or, for data observed\
  \ on a regular transect or grid, with Fourier spectral randomization methods that\
  \ can flexibly model spatial structure at any scale. This study uses Moran eigenvector\
  \ maps to extend spectral randomization to irregularly spaced samples. We present\
  \ different algorithms to perform restricted randomization to suit different types\
  \ of research questions: individual randomization of each variable, joint randomization\
  \ of a group of variables while keeping within-group correlations fixed, and randomization\
  \ with a fixed correlation between original data and randomized replicates (e.g.\
  \ as input for simulation studies). The performance of the proposed Moran spectral\
  \ randomization methods for regularly and irregularly spaced samples is assessed\
  \ with correlation analysis of simulated data. Moran spectral randomization closely\
  \ matched the spatial structure of original simulated data sets, with identical\
  \ or nearly identical Moran's I values and power spectra, depending on the algorithm.\
  \ In correlation analysis of two spatially autocorrelated variables, Moran spectral\
  \ randomization produced correct type I error rates for stationary spatial data,\
  \ even for very small and highly irregular samples, but was sensitive to linear\
  \ trend. When one or both variables lacked spatial structure, Moran spectral randomization\
  \ tests were more conservative than correlation t-tests. The proposed Moran spectral\
  \ randomization method requires a minimum of parameterization and is able to address\
  \ multivariate data with spatial structure at multiple scales, with the option of\
  \ controlling levels of correlation with the original data. It can provide technically\
  \ unlimited numbers of randomizations even for small samples while closely maintaining\
  \ the spatial characteristics of uni- or multivariate data at all spatial scales.\
  \ The method is applicable for correlation analysis of stationary, autocorrelated\
  \ spatial or temporal series. Further research should assess whether the method\
  \ can be extended to multiple regression analysis."
publication: '*Methods in Ecology and Evolution*'
doi: 10.1111/2041-210X.12407
---
