# Spatio-Temporal Traffic Demand Prediction Engine (Flipkart GRiD)

This repository contains an end-to-end Machine Learning pipeline developed to solve the Traffic Demand Prediction challenge from the Flipkart GRiD Hackathon. The objective is to forecast hyperlocal transport demand by analyzing complex geospatial, environmental, and infrastructure data.

## Project Highlights
- **Engineered Features:** Extracted structural insight from `geohash` spatial data, computed target encodings for categorical variables (`Weather`, `RoadType`), and isolated cyclical temporal trends from timestamps.
- **Model Benchmark & Selection:** Built and evaluated multiple advanced regression architectures using 5-Fold Cross-Validation:
  - **Random Forest Regressor: 0.86697 (Best Performance)**
  - XGBoost Regressor: 0.85627
  - LightGBM Regressor: 0.85270
  - CatBoost Regressor: 0.82472
- **Key Metric:** Achieved an $R^2$ validation score of **86.7%**, mapping out to a high-tier efficiency rating under the competition's evaluation metric: `max(0, 100 * r2_score)`.

## Repository Contents
- `traffic_demand_prediction.ipynb`: Full notebook containing data preprocessing, exploratory analysis, feature extraction, cross-validation, and model training.
- `submission.csv`: Final output predictions matching the test dataset indices.
