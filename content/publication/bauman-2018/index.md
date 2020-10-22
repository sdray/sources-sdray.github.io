---
# Documentation: https://wowchemy.com/docs/managing-content/

title: Disentangling Good from Bad Practices in the Selection of Spatial or Phylogenetic
  Eigenvectors
subtitle: ''
summary: ''
authors:
- David Bauman
- Thomas Drouet
- Stéphane Dray
- Jason Vleminckx
tags:
- '"akaike information criterion (aic)"'
- '"ecological processes"'
- '"eigenvector selection"'
- '"forward selection"'
- "\"moran's eigenvector maps (mem)\""
- '"phylogenetic eigenvector regression (pvr)"'
- '"principal coordinates of neighbour matrices (pcnm)"'
- '"spatial eigenvector mapping (sevm)"'
- '"spatial patterns"'
- '"variation partitioning"'
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
publishDate: '2020-10-22T18:41:03.974918Z'
publication_types:
- '2'
abstract: 'Eigenvector mapping techniques are widely used by ecologists and evolutionary
  biologists to describe and control for spatial and/or phylogenetic patterns in their
  data. The selection of an appropriate subset of eigenvectors is a critical step
  (misspecification can lead to highly biased results and interpretations), and there
  is no consensus yet on how to proceed. We conducted a ten-year review of the practices
  of eigenvector selection and highlighted three main procedures: selecting the subset
  of descriptors minimising the Akaike information criterion (AIC), using a forward
  selection with double stopping criterion after testing the global model significance
  (FWD), and selecting the subset minimising the autocorrelation in the model residuals
  (MIR). We compared the type I error rates, statistical power, and R$^2$ estimation
  accuracy of these methods using simulated data. Finally, a real dataset was analysed
  using variation partitioning analysis to illustrate to what extent the different
  selection approaches affected the ecological interpretation of the results. We show
  that, while the FWD and MIR approaches presented a correct type I error rate and
  were accurate, the AIC approach displayed extreme type I error rates (100%), and
  strongly overestimated the R$^2$. Moreover, the AIC approach resulted in wrong ecological
  interpretations, as it overestimated the pure spatial fraction (and the joint spatial-environmental
  fraction to a lesser extent) of the variation partitioning. Both the FWD and MIR
  methods performed well at broad and medium scales but had a very low power to detect
  fine-scale patterns. The FWD approach selected more eigenvectors than the MIR approach
  but also returned more accurate R$^2$ estimates. Hence, we discourage any future
  use of the AIC approach, and advocate choosing between the MIR and FWD approaches
  depending on the objective of the study: controlling for spatial or phylogenetic
  autocorrelation (MIR) or describing the patterns as accurately as possible (FWD).'
publication: '*Ecography*'
doi: 10.1111/ecog.03380
---
