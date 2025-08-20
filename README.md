# IPL Match Outcome Prediction and Player Role Segmentation

## Overview
This project forms part of my MSc Data Science dissertation at the University of Sheffield. 
It develops an interpretable machine learning framework for:

1. Pre-toss IPL match outcome prediction using pre-match performance, contextual, and team-composition features.  
2. Unsupervised player role segmentation for batters and bowlers based on recent performance trends.  

The study uses ball-by-ball data from multiple IPL seasons (sourced from public Kaggle datasets) and applies both supervised and unsupervised learning techniques to deliver predictive and diagnostic insights.

---

## Research Questions (RQs)
RQ1: Can unsupervised learning techniques be used to define interpretable, role-based player clusters (e.g., top-order anchors, finishers, strike bowlers) using rolling and phase-specific performance data?

RQ2: To what extent can IPL match outcomes be predicted using pre-match contextual features, such as venue effects, team composition, player form, momentum, and head-to-head strength indicators?

RQ3: To what extent does momentum (measured via recent win rate differentials) matter in IPL, and do teams with higher recent win rates tend to win more matches?

RQ4: How do aggregated team-level metrics constructed from clustered player roles and recent form influence match outcomes, based on statistical testing?

## Repository Contents
- **IPL.ipynb**  
  Main Jupyter notebook containing:  
  - Data cleaning & preprocessing  
  - Feature engineering  
  - Clustering pipeline (player role segmentation)  
  - Team-level aggregation  
  - Train-test split  
  - Model training (Random Forest, XGBoost, CatBoost, Logistic Regression baseline)  
  - Model evaluation & visualisation  

- **README.md**  
  This file – setup, execution, and project description.  

---

## Data Availability
The raw datasets are **not included in this repository** due to size constraints. They can be downloaded directly from Kaggle:  

- [matches.csv](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020?select=matches.csv)  
- [deliveries.csv](https://www.kaggle.com/datasets/patrickb1912/ipl-complete-dataset-20082020?select=deliveries.csv)  

Once downloaded, place both files in the same folder as this README and the notebook (`IPL.ipynb`) before running.

---

## Requirements
Python 3.12.4 with the following core libraries:  
- pandas  
- numpy  
- scikit-learn  
- matplotlib  
- seaborn  
- xgboost  
- catboost  
- shap  

---

## Running the Notebook
1. Clone or download this repository.
2. Download the raw CSV files from Kaggle and place them alongside this README and `IPL.ipynb`.  
3. Open `IPL.ipynb` in Jupyter Lab or Jupyter Notebook.  
4. Run all cells sequentially to:  
   - Prepare and clean the data  
   - Generate engineered features  
   - Train the models  
   - View evaluation metrics and visualisations  

---

## Notes
- Reproducibility: A fixed random seed is used in modelling steps for consistency.  
