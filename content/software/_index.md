---
# Documentation: https://wowchemy.com/docs/managing-content/

title: "Software"
subtitle: ""
summary: ""
authors: []
tags: []
categories: []
date: 2020-11-03T17:11:18+01:00
lastmod: 2020-11-03T17:11:18+01:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---
An important part of my activity is devoted to the development of statistical software, mainly {{< icon name="r-project" pack="fab" >}} packages. I contribute to the following projects and occasionally to other packages (e.g., Guerry, spdep, adehabitat). Development versions of the packages are available on my GitHub page. 

## `ade4`

The ade4 package provides statistical tools and graphical functions for the analysis of multivariate data. It contains methods for the analysis of one table (principal component analysis, correspondence analysis, multiple correspondence analysis, etc.), a pair of tables (coinertia analysis, redundancy analysis, canonical correspondence analysis, etc.) or multiple tables (partial triadic analysis, STATIS, multiple coinertia analysis, etc.). 

## `adespatial`

The package adespatial contains functions for the multiscale analysis of spatial multivariate data. It implements some new functions and reimplements existing functions that were available in packages of the sedaR project hosted on R-Forge (spacemakeR, packfor, AEM, etc.).

## `adephylo`

The package adephylo provides tools for quantifying and describing the phylogenetic structures of biological traits. It implements tests of phylogenetic signal, phylogenetic distances and proximities, and novel methods for describing further univariate and multivariate phylogenetic structures. 

## `adegraphics`  

This package is a complete reimplementation of the graphical functionalities of ade4. It uses the lattice package as a framework and an S4 object-oriented approach. It handles simple and multiple graphics to produce publication-quality figures.

## `ade4TkGUI`

ade4TkGUI provides a graphical user interface for some basic functions (data import, basic multivariate methods, two-table methods, etc.) of the multivariate data analysis package ade4. The aim of this interface is to make the use of the ade4 package easier, particularly for beginners or occasional users. 
