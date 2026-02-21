# London Schools – Exploratory, Spatial & Cluster Analysis

## Project Overview

This project performs an **exploratory data analysis (EDA)** and **spatial analysis** of schools in London.  
The dataset contains **2,166 observations and 29 variables**, combining school-level characteristics with regional socio-economic indicators.

The data includes:
- School attributes (school type, attainment rates, Ofsted ratings)
- Geographic information (longitude, latitude, borough)
- Regional indicators (income scores, crime scores)

The analysis aims to identify **data quality issues**, **spatial patterns**, and **clusters of similar schools**, and to assess whether **dimensionality reduction** can reveal additional structure in the data.

---

## Objectives

- Assess data quality by identifying missing values and anomalies
- Apply data cleaning and imputation techniques
- Perform spatial analysis of schools across London boroughs
- Identify clusters based on numeric school and regional features
- Apply **Principal Component Analysis (PCA)** to reduce dimensionality
- Evaluate whether PCA improves cluster separation and interpretability

---

## Data Sources

### Primary Dataset
- `london_schools_data.csv`
  - Contains school characteristics, performance indicators, and regional metrics

### Geographic Data
- ESRI shapefile:
  - `ESRI/London_Borough_Excluding_MHW.shp`
  - Used for borough-level spatial visualization and mapping

---

## Technologies & Libraries Used

This project is implemented in **R** using the following packages:

### Data Manipulation & Utilities
- dplyr
- purrr
- lubridate

### Visualization
- ggplot2
- ggpubr
- gridExtra
- GGally
- corrplot
- patchwork
- ggrepel

### Missing Data Handling
- naniar
- MissMech
- mice

### Spatial Analysis
- sf

### Time Series & Statistical Tools
- tseries

### Clustering & Dimension Reduction
- cluster
- factoextra

---

## Environment Setup

To install the required packages, run:

```r
install.packages(c(
  "ggplot2", "tseries", "gridExtra", "dplyr", "corrplot",
  "ggpubr", "GGally", "lubridate", "naniar", "sf",
  "MissMech", "mice", "cluster", "factoextra",
  "purrr", "patchwork", "ggrepel"
))
