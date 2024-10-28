
---
title: "README - TB Incidence in East Africa"
author: "Your Name"
format: markdown
---

# Overview

This project examines the incidence and distribution of tuberculosis (TB) cases across East African countries. The data visualization provides a geographic representation of TB cases, highlighting country-specific variations and identifying areas with higher disease burdens. This analysis aids in understanding the regional impact of TB and supports efforts toward targeted interventions.

## Objectives

The primary objectives of this project are:

1. **Geographic Visualization**: To provide a clear, map-based view of TB case distribution across East African countries.
2. **Case Ranges by Country**: To categorize countries based on ranges of TB cases, aiding in easy identification of high-incidence areas.
3. **Policy Support**: To offer insights for policy-makers on where to focus healthcare resources for TB prevention and treatment.

## Data Sources

- **Geographic Boundaries**: The boundaries data for countries were obtained from [GeoJSON World Boundaries](https://github.com/datasets/geo-boundaries-world-110m).
- **TB Cases Data**: This project uses a dataset that includes TB case counts for East African countries, with fields for each country's name and the number of estimated cases (denoted as `best` for "best estimate" of cases).

## Methodology

1. **Data Collection**: The dataset contains geographic information on East African countries and TB incidence data.
2. **Data Cleaning**: Geographic data was filtered to include only East African countries. Then, TB incidence data was merged with geographic data to create a unified dataset for visualization.
3. **Classification of TB Cases**: TB case counts are grouped into ranges for improved visualization. This classification simplifies understanding of TB burdens across regions.
4. **Map Visualization**: Using Python's `matplotlib` and `geopandas`, a choropleth map visualizes TB cases with color-coded ranges for each country. Each range is displayed in the legend for easy interpretation.

## Visualization

A choropleth map represents TB case distribution across East African countries. The legend categorizes TB cases into the following ranges:

- **13,990 - 90,000**: Countries with lower incidence rates.
- **90,001 - 170,000**: Moderate TB incidence.
- **170,001 - 250,000**: High TB incidence.

Each country is color-coded based on its TB case range, and country names are annotated at the centroid of each geographic area for clarity.

## Results

The map visualization indicates varying TB incidence across East Africa. Countries with higher TB burdens are more visually prominent, allowing stakeholders to quickly identify regions with more significant healthcare needs related to TB.

## Technical Implementation

This project is implemented in Python using the following key libraries:

- **GeoPandas**: For handling and visualizing geographic data.
- **Matplotlib**: For creating the choropleth map.
- **Pandas**: For data manipulation and range categorization of TB cases.

## Available Formats

- [View HTML Version](https://htmlpreview.github.io/?https://github.com/analystnyamu/TB-Article/blob/master/TB-Article.html)
- [Download PDF Version](TB-Article.pdf)

### Key Code Snippets

The following snippet categorizes TB cases into defined ranges and visualizes the map with color-coded ranges:

```python
import geopandas as gpd
import pandas as pd
import matplotlib.pyplot as plt

# Load and merge data, categorize TB cases into ranges, and plot
# ...

# Define ranges and labels
bins = [13990, 90000, 170000, 250000]
labels = ["13,990-90,000", "90,001-170,000", "170,001-250,000"]
east_africa_tb_data["case_range"] = pd.cut(east_africa_tb_data["best"], bins=bins, labels=labels)

# Plot data
# ...



