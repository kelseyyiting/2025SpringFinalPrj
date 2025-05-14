# Analysis of Bicycle Accident Patterns in Chicago

## Project Overview

This repository contains code and data for analyzing bicycle crashes in Chicago, comparing privately owned bicycles and Divvy rental bikes (classic vs. electric). Key aims:
- Assess crash frequency and severity by vehicle type
- Investigate the effect of rider age and time of day on injury outcomes
- Visualize spatial hotspots for owned vs. rental crashes
- Perform regression to test the relationship between rider age and no-injury rates
  
## Data Sources

- Traffic Crashes – People (2022–2024): crash records with information about the people involved. https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if/about_data
- Traffic Crashes - Crashes(2022-2024): crash records with detailed location and description. https://data.cityofchicago.org/Transportation/Traffic-Crashes-Crashes/85ca-t3if/about_data
- Divvy Trip Data: Divvy ridership records https://divvybikes.com/system-data

## Key Python packages:
- pandas, numpy, geopandas
- matplotlib, seaborn
- scikit-learn
- statsmodels, scipy
- contextily (for basemap)

## Running the Analysis
1. Data Preparation & Descriptive StatisticsOpen finalprj.ipynb and run cells for data loading, cleaning, and initial summaries.
2. Time‑Series & Regression
  - Monthly and hourly trends plots
  - Regression of age vs. no‑injury rate (slopes, p‑values, R²)
3. Hotspot MappingExecute scripts/hotspot_analysis.py to generate KDE contour maps for owned vs. rental crashes.
4. SlidesThe presentation in slides/Analysis of Bicycle Accident Patterns in Chicago.pptx summarizes motivation, methods, results, and demo plan.
