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
  - hourly trends plots
  - Regression of age vs. no‑injury rate (slopes, p‑values, R²)
3. Hotspot MappingExecute scripts/hotspot_analysis.py to generate KDE contour maps for owned vs. rental crashes.
4. SlidesThe presentation in slides/Analysis of Bicycle Accident Patterns in Chicago.pptx summarizes motivation, methods, results, and demo plan.

## Results Summary
- Owned vs. Rental Crashes: 6,574 vs. 122 (98.2% vs. 1.8%).
- Rental Breakdown: classic (54%), electric (43%), others (3%).
- Regression: Age vs. No‑Injury Rate shows a negative slope (~–0.005 per year), p < 0.01, R² ≈ 0.40.
 ![image](https://github.com/user-attachments/assets/d26019fa-ff59-4c4a-9afb-1dfc59c8b8f4)
 ![image](https://github.com/user-attachments/assets/a14f5f67-d3dd-4b2e-9cd2-e7bdc0ede196)
- Spatial KDE: distinct high-crash hotspots mapped for owned and rental bikes.
![image](https://github.com/user-attachments/assets/1e5e6843-31b8-403e-8dcf-8b64ae2ec521)
