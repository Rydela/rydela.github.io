---
layout: project
title: "Automated Humanitarian Data Classification"
slug: "automated-humanitarian-data-classification"
year: 2021
section: "Natural Language Processing"
summary: "NLP classification pipeline to auto-tag humanitarian datasets and reduce manual triage in emergency data workflows."
methods:
  - Python
  - FastText embeddings
  - Multi-layer perceptron
  - Supervised classification
outcome: "Reached 91.8% average classification accuracy across key humanitarian data categories used in rapid assessments."
status: "archived"
image: "/assets/images/projects/humdata/humdata3.png"
organization:
  name: "Humanitarian Data Exchange"
  url: "https://data.humdata.org/"
links:
  - label: "GitHub"
    url: "https://github.com/Rydela/Humanitarian-Data-Classification"
  - label: "Organization"
    url: "https://data.humdata.org/"
---
### Problem
Large volumes of crisis data arrive with inconsistent metadata, making category assignment and prioritization slow for response teams.

### Work
I built a training dataset from scraped HDX resources, engineered text features, and trained a neural classifier to infer category labels from content patterns.

### Delivery
The resulting workflow demonstrated strong automated triage potential for humanitarian information management pipelines.
