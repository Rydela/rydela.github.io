---
layout: project
title: Automated Humanitarian Data Classification
permalink: /projects/automated-humanitarian-data-classification/
date: 2021-01-15
categories: [projects]
project:
  summary: NLP classification pipeline to auto-tag humanitarian datasets and reduce manual triage in emergency data workflows.
  methods:
    - Python
    - FastText embeddings
    - Multi-layer perceptron
    - Supervised classification
  outcome: Reached 91.8% average classification accuracy across key humanitarian data categories used in rapid assessments.
  status: archived
  featured: true
  category: machine-learning
organization:
  name: Humanitarian Data Exchange
  url: https://data.humdata.org/
links:
  - label: GitHub Repository
    url: https://github.com/Rydela/Humanitarian-Data-Classification
---
### Problem
Large volumes of crisis data arrive with inconsistent metadata, making category assignment and prioritization slow for response teams.

### Work
I built a training dataset from scraped HDX resources, engineered text features, and trained a neural classifier to infer category labels from content patterns.

### Delivery
The resulting workflow demonstrated strong automated triage potential for humanitarian information management pipelines.
