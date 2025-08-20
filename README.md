IPL Match Outcome Prediction and Player Role Segmentation

#Overview
This project is part of my MSc dissertation at the University of Sheffield, supervised by Professor Val Gillet.
It develops an interpretable machine learning framework for:
1. Pre-toss IPL match outcome prediction using pre-match performance, contextual, and team-composition features.
2. Unsupervised player role segmentation for batters and bowlers based on recent performance trends.
The study uses ball-by-ball data from multiple IPL seasons (sourced from public Kaggle datasets) and applies both supervised and unsupervised learning techniques to deliver predictive and diagnostic insights.

#Repository Contents
- IPL.ipynb
  Main Jupyter notebook containing:
  - Data cleaning & preprocessing
  - Feature engineering
  - Clustering pipeline (player role segmentation)
  - Team-level aggregation
  - Train-test split
  - Model training (Random Forest, XGBoost, CatBoost, Logistic Regression baseline)
  - Model evaluation & visualisation

- Data files
  - matches.csv : raw match-level dataset
  - deliveries.csv : ball-by-ball data
  - cleaned_matches.csv : cleaned and processed match-level dataset
  - cleaned_deliveries.csv : cleaned and processed ball-by-ball dataset
  - batting_rolling_metrics.csv : rolling performance metrics for batters
  - bowling_rolling_metrics.csv : rolling performance metrics for bowlers
  - match_features_final.csv : engineered dataset for modelling

- README.md
  This file - describing setup, execution, and file structure.

#Requirements
The project uses Python 3.12.4 with the following core libraries:
  - pandas
  - numpy
  - scikit-learn
  - matplotlib
  - seaborn
  - xgboost
  - catboost
  - shap

#Running the Notebook
  1. Clone or download the project folder.
  2. Ensure the raw CSV files (matches.csv and deliveries.csv) are in the same folder as this README and IPL.ipynb.
  3. Open IPL.ipynb in Jupyter Lab or Jupyter Notebook.
  4. Run all cells sequentially to:
     - Prepare and clean the data
     - Generate engineered features
     - Train the models
     - View evaluation metrics and visualisations

#Notes
  - Data Source: The dataset was sourced from publicly available IPL ball-by-ball records on Kaggle.
  - Reproducibility: A fixed random seed is set in all modelling steps to ensure consistent results.
  - Ethics: This work uses only secondary and publicly available data.