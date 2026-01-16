# predictive-maintenance-ml
Predictive maintenance using machine learning to estimate machine failure probability
# Predictive Maintenance Using Machine Learning

## Project Overview
This project focuses on predicting machine failures using historical sensor and operational data. 
The goal is to estimate the probability of machine failure under given operating conditions to enable preventive maintenance.

## Problem Statement
Unplanned machine failures lead to downtime, financial losses, and safety risks. 
This project applies machine learning to identify failure patterns and support data-driven maintenance decisions.

## Dataset
The dataset contains sensor measurements such as:
- Air temperature
- Process temperature
- Rotational speed
- Torque
- Tool wear
- Machine type

Target variable:
- Machine failure (0 = No failure, 1 = Failure)

## Approach
- Data cleaning and exploratory data analysis
- Feature engineering and data preparation
- Logistic Regression modeling
- Model evaluation using confusion matrix and probability thresholds
- Business interpretation of results

## Results
The model achieved high predictive performance and effectively identified failure-prone conditions. 
Threshold tuning was used to balance between missed failures and false alarms.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn
- Matplotlib, Seaborn

## Conclusion
This project demonstrates an end-to-end predictive maintenance workflow and highlights how machine learning supports preventive maintenance strategies.
