---
# Documentation: https://wowchemy.com/docs/managing-content/

title: 'Being confident in confidence scores: calibration in deep learning models
  for camera trap image sequences'
subtitle: ''
summary: ''
authors:
- Gaspard Dussert
- Simon Chamaillé-Jammes
- Stéphane Dray
- Vincent Miele
tags:
- Calibration
- camera trap
- confidence score
- interpretability
- machine learning
- species classification
categories: []
date: '2024-01-01'
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
publishDate: '2024-09-09T09:27:35.376570Z'
publication_types:
- '2'
abstract: In ecological studies, machine learning models are increasingly being used
  for the automatic processing of camera trap images. Although this automation facilitates
  and accelerates the identification step, the results of these models may lack interpretability
  and their immediate applicability to ecological downstream tasks (e.g. occupancy
  estimation) remains questionable. In particular, little is known about their calibration,
  a property that allows confidence scores to be interpreted as probabilities that
  model's predictions are true. Using a large and diverse European camera trap dataset,
  we investigate whether deep learning models for species classification in camera
  trap images are well calibrated. Additionally, as camera traps are often configured
  to take multiple photos of the same event, we also explore the calibration of predictions
  aggregated across sequences of images. Finally, we study the effect and the practicality
  of a post-hoc calibration method, i.e. temperature scaling, for predictions made
  at image and sequence levels. Based on five established models and three independent
  test sets, we show that averaging the logits over the sequence, selecting an appropriate
  architecture, and optionally using temperature scaling can produce well-calibrated
  models. Our findings have clear implication for, for instance, the calculation of
  error rates or the selection of confidence score thresholds in ecological studies
  making use of artificial intelligence models.
publication: '*Remote Sensing in Ecology and Conservation*'
doi: 10.1002/rse2.412
links:
- name: URL
  url: https://onlinelibrary.wiley.com/doi/abs/10.1002/rse2.412
---
