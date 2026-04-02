# Case Study: Web Scraping and Country Data Analysis

## Problem

Many beginner analytics projects start from a ready-made CSV. In real work, that is often not enough. The goal of this project was to show that I can collect public data from the web, clean inconsistent fields, merge multiple sources, and build an analysis-ready dataset.

## Data Sources

- Worldometer population by country page using `2026` population estimates
- Worldometer GDP by country page using `2025` IMF-based nominal GDP projections

## Workflow

1. Sent HTTP requests to both source pages.
2. Parsed HTML tables into pandas DataFrames.
3. Cleaned currency, percentage, comma-separated, and missing-value fields.
4. Standardized country names so the tables could be merged correctly.
5. Built a unified country-level dataset and generated charts.

## Results

- merged `218` country-level rows
- created reusable raw HTML snapshots and raw CSV extractions
- built a processed country analysis dataset ready for further EDA or modeling

## Example Insights

- Country size and GDP rank are often very different, which shows why population alone is not enough to understand economic scale.
- Urbanization and GDP per capita display a broad positive relationship with clear outliers.
- The project creates a base dataset that can support future analysis in policy, business, education, or macroeconomic contexts.

## What This Shows About Me

- I can collect my own dataset instead of depending only on provided files.
- I can clean real-world messy web data into structured tables.
- I can connect data collection work to analysis and presentation.
