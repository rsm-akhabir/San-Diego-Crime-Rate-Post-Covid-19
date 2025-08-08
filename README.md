# Project Overview
This project presents a comprehensive, data-driven framework for analyzing and forecasting crime patterns in San Diego using the National Incident-Based Reporting System (NIBRS) data. Spanning 2020 to the present, the dataset captures detailed information on crime type, time, location, and context. The project aims to support smarter policing strategies through temporal trend analysis, geospatial heatmaps, and predictive modeling of crime incidents—especially in light of disruptions caused by COVID-19.

# Methods
The analysis integrates exploratory data analysis, spatial mapping, and predictive machine learning:

Trend Analysis: Monthly and annual breakdowns of crime by category (Property, Society, Personal) identify fluctuations pre-, during-, and post-COVID.

Geospatial Heatmaps: Visualize neighborhood-level crime concentrations to inform targeted policing.

Random Forest Regression: Predicts future crime counts based on temporal, categorical, and contextual variables, achieving an R² of 0.92.

# Data Preparation
Dataset: NIBRS San Diego incident-level data (2020–2024)

# Cleaning & Structuring:

- Filtered crime records for valid geographic coordinates and high geocoding confidence

- Standardized and categorized offenses by type (Property, Society, Personal)

- Added temporal features (month, day of week, hour) and lockdown/event labels

# Feature Engineering:

- Labeled lockdown phases and major public events

- Aggregated data by neighborhood, crime category, and time window

- Added derived fields like "crime against" group and contextual markers for public holidays

# Evaluation & Results
Key Findings:

- Most common crimes: Group B, Larceny/Theft, and Assault offenses

- Highest crime concentration: East Village (10,865+ incidents), followed by Pacific Beach

- COVID-19 effect: Sharp drop in early lockdown, followed by a rebound; property crimes remained the most persistent category

- Event impact: Major holidays had significantly fewer incidents—possibly due to increased policing or public caution

# Model Performance:

- Random Forest Regressor achieved an R² of 0.92, effectively capturing seasonal and pandemic-related fluctuations

- Top predictive features included month, crime type, and lockdown status

# Financial and Public Safety Relevance
- By identifying high-crime neighborhoods and forecasting future hotspots, this project helps optimize:

- Police deployment strategies (e.g., during late-night hours, weekends, or known peak months)

- Surveillance planning near transit hubs and downtown

- Post-COVID community support initiatives to address property crimes driven by economic stress

Tech Stack: Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Leaflet (map visualization), Jupyter Notebook

# Key Outcomes: 

- Delivered a predictive crime model with 92% accuracy

- Identified critical hotspots and high-risk timeframes

- Demonstrated the value of using public event tagging and lockdown status in forecasting

- Supported policy decisions with data-backed evidence on when and where to deploy resources
