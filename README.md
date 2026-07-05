# Global Tourism Patterns and Visitor Behaviour in Dubai

A data visualization project analyzing international tourism from two angles: country-level arrival trends worldwide (1960-2020), and individual traveler behavior in the United Arab Emirates. Built in R using tidyverse and ggplot2.

## Overview

This project combines two datasets that complement each other:

- **World Bank tourism arrivals data** — international visitor arrivals by country, 1960-2020. Used to examine tourism at a global scale (rankings, trends over time, geographic distribution).
- **UAE tourism behavior dataset (Kaggle)** — 1,000 individual traveler records covering country of origin, travel purpose, accommodation type, length of stay, and spending. Used to examine visitor behavior at an individual level.

## Research questions

- Which countries received the most foreign visitors in 2016, and how have arrivals changed over time for specific countries?
- How does accommodation choice vary by travel purpose?
- How does average length of stay differ across the most common countries of origin?
- What patterns exist between travel purpose and country of origin?

## Visualizations produced

1. World choropleth map of 2016 arrivals
2. Top 15 countries by arrivals
3. Arrivals over time (selected countries)
4. Sankey-style plot: travel purpose vs. accommodation type
5. Average stay duration by tourist origin
6. Heatmap: tourist origin vs. travel purpose

## Key findings

Foreign arrivals are concentrated in a relatively small number of countries, with France leading global arrivals. Growth trends vary substantially by country — India and the UAE show particularly strong increases over the period studied. Within the UAE dataset, average stay duration is fairly similar across major origin countries, spending varies only slightly by accommodation type, but accommodation choice varies significantly by travel purpose. Tourist origin and travel purpose combinations are spread across many categories rather than dominated by one clear pattern — together, the visualizations show tourism can be understood both geographically and behaviorally.

## Tech stack

R, tidyverse, sf, rnaturalearth, ggalluvial, RColorBrewer, viridis, R Markdown

## Files

- `Assignment.Rmd` — R Markdown source (all code and analysis)
- `Assignment.nb.html` — rendered notebook (open in any browser, no R installation needed)
- `API_ST_INT_ARVL_DS2_en_csv_v2_1927083.csv` — World Bank tourism arrivals dataset
- `tourism_behavior_analysis_updated_data.xlsx` — UAE individual traveler dataset

## Running it yourself

Requires R and RStudio. Open `Assignment.Rmd` in RStudio and install the required packages if needed:

```r
install.packages(c("tidyverse", "readxl", "sf", "rnaturalearth",
                    "rnaturalearthdata", "scales", "RColorBrewer",
                    "viridis", "ggalluvial"))
```

Then click **Knit** to reproduce the full report and all visualizations.

## Data sources

- World Bank tourism arrivals: https://data.worldbank.org/indicator/ST.INT.ARVL
- UAE tourism behavior dataset (Kaggle): https://www.kaggle.com/datasets/muhamamdumeraliriaz/tourism-behavior-analysis-in-uae
- Natural Earth world map data: https://www.naturalearthdata.com/
