---
layout: project
title: "Overture Link Data Pipeline"
slug: "overture-link-data-pipeline"
year: 2025
section: "Data Engineering"
summary: "Open-source ETL pipeline published for the World Bank to automate Overture Maps extraction, transformation, and publishing across operational geospatial workflows."
methods:
  - Python CLI
  - ETL automation
  - Geospatial data engineering
  - DuckDB-based querying
  - ArcGIS Online integration
outcome: "Reduced manual geospatial processing time through a repeatable workflow supporting 176 countries, reusable queries, and both ArcGIS Online publishing and portable GIS exports."
status: "complete"
organization:
  name: "World Bank"
  url: "https://github.com/worldbank"
links:
  - label: "GitHub"
    badge_message: "View on GitHub"
    url: "https://github.com/worldbank/OvertureLink-Data-Pipeline"
  - label: "Organization"
    badge_message: "Visit World Bank"
    url: "https://github.com/worldbank"
---
### Problem
Teams often spend significant time repeating the same geospatial data preparation steps across countries, tools, and reporting cycles.

### Work
I developed and published an open-source pipeline with modular Source -> Transform -> Publish/Export stages, including CLI commands for cached Overture dumps (`overture-dump`), ArcGIS Online publishing (`arcgis-upload`), and direct file export (`export`).

### Delivery
The result is a reusable World Bank-ready workflow that scales across countries and sectors, shortens setup time for new analyses, and improves consistency for recurring production geospatial pipelines.
