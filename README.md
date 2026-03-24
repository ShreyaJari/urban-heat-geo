# urban-heat-geo
GeoAI workflow for urban heat island mapping and vulnerability analysis using Earth observation and machine learning.

# Urban Heat Island and Vulnerability Analysis using Earth Observation and Machine Learning

## Project Overview

This project explores urban heat island patterns using Earth observation and urban geospatial variables, with a focus on building an interpretable GeoAI workflow for city-scale heat analysis. The goal is to map urban heat, identify hotspots, and understand which environmental and built-up factors are most strongly associated with higher surface temperatures.

This project is part of my broader GeoAI and Earth Observation portfolio focused on environmental intelligence, climate-related risk, and interpretable machine learning for Earth systems.

---

## Why This Project Matters

Urban heat is one of the most visible and harmful effects of rapid urbanization and climate change. Built-up surfaces, reduced vegetation, and changing land cover can intensify heat in cities, increasing health risk, discomfort, energy demand, and vulnerability.

Understanding where urban heat is concentrated and what drives it can support:
- urban climate resilience
- better planning and mitigation
- greener infrastructure strategies
- environmental intelligence workflows for cities

---

## Research Question

**Can satellite-derived thermal, vegetation, land cover, and built-environment indicators be used to model and explain urban heat island intensity at city scale?**

---

## Study Area

**Nagpur, India**

Nagpur is used as the first case-study city because of its hot climate, growing urban footprint, and relevance to heat stress in Indian urban environments.

---

## Project Objectives

This project aims to:

- map land surface temperature (LST) across the study area
- identify urban heat hotspots
- derive environmental and built-up explanatory features
- model urban heat patterns using machine learning
- interpret which variables are most strongly associated with hotter areas
- create clear visual outputs for research communication and portfolio presentation

---

## Target Variable

### Primary Target
- **Land Surface Temperature (LST)**

### Optional Secondary Target
- **Heat hotspot class** (hotspot vs non-hotspot)

The main workflow is designed around predicting or explaining continuous heat intensity using LST.

---

## Candidate Input Features

Potential explanatory variables include:

- NDVI (Normalized Difference Vegetation Index)
- NDBI (Normalized Difference Built-up Index)
- land cover / land use
- vegetation cover
- built-up density
- water mask / proximity to water
- elevation
- impervious surface proxy
- population density *(optional, if included in later versions)*

---

## Data Sources

Planned or candidate datasets include:

- **Landsat 8 / Landsat 9** for thermal bands and LST-related analysis
- **Sentinel-2** for vegetation and built-up indices
- **SRTM / DEM** for elevation
- **Land cover datasets** for urban, vegetation, and water classes
- optional urban or population datasets for vulnerability context

Final datasets used in the project will be listed and documented clearly as the workflow is completed.

---

## Methodology

The project will be developed in the following stages:

### 1. Data Preparation
- define the study area boundary
- collect and preprocess satellite and geospatial data
- align spatial layers to a consistent extent and resolution
- derive remote sensing indices such as NDVI and NDBI

### 2. Urban Heat Mapping
- derive or estimate land surface temperature
- generate city-scale heat maps
- identify heat hotspot zones

### 3. Exploratory Spatial Analysis
- examine relationships between LST and vegetation, built-up area, water, and elevation
- visualize spatial patterns and feature distributions

### 4. Machine Learning
- train baseline and stronger regression models to explain or predict LST
- compare model performance across selected features

### 5. Explainability and Interpretation
- analyze feature importance
- apply SHAP if feasible
- interpret which variables contribute most to heat intensity
- discuss why certain parts of the city are hotter than others

---

## Planned Models

### Baseline Model
- **Random Forest Regressor**

### Advanced Model
- **XGBoost Regressor**

These models are selected because the primary target, LST, is continuous.

---

## Explainability

Interpretability is a key part of this project.

Planned explainability components include:
- feature importance plots
- SHAP analysis *(if feasible)*
- comparison of major heat drivers
- discussion of spatial heat patterns in relation to vegetation and built-up area

---

## Expected Outputs

This project is expected to produce:

- urban heat map for Nagpur
- hotspot map
- feature relationship analysis
- machine learning model evaluation metrics
- feature importance / SHAP visualizations
- GitHub-ready figures and documentation
- LinkedIn-ready visual summary of findings

---

## Skills Demonstrated

This project is designed to showcase:

- Earth Observation analysis
- geospatial data processing
- remote sensing feature engineering
- urban climate intelligence
- machine learning for environmental data
- interpretable AI
- research-style project communication
- GitHub portfolio development

---

## Project Structure

```text
urban-heat-geoai/
│── README.md
│── requirements.txt
│── environment.yml
│── .gitignore
│── data/
│   ├── raw/
│   ├── processed/
│── notebooks/
│── src/
│   ├── data/
│   ├── features/
│   ├── models/
│   ├── evaluation/
│   ├── visualization/
│── results/
│   ├── figures/
│   ├── maps/
│   ├── metrics/
│── docs/
