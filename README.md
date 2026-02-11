 Predictive Maintenance using Machine Learning
Project Overview

Unexpected machine failures can cause production downtime, increase maintenance costs, and reduce operational efficiency. This project develops a machine learning model to predict the probability of machine failure using sensor data collected from industrial equipment.

The objective is to support predictive maintenance, allowing companies to detect potential failures early and perform maintenance before breakdowns occur.

 Project Goals

Predict whether a machine is likely to fail

Identify important factors contributing to machine failure

Evaluate model performance using multiple metrics

Analyze decision thresholds for real industrial application

Demonstrate business value of predictive maintenance systems

Dataset

The dataset contains sensor and operational data from industrial machines. Each row represents machine operating conditions at a specific time.

Features include:

Air temperature

Process temperature

Rotational speed

Torque

Tool wear

Machine type

Target Variable:

Machine Failure

0 → No failure

1 → Failure

 Methodology
 Exploratory Data Analysis (EDA)

Investigated feature distributions

Checked for missing values

Analyzed class imbalance

Explored relationships between sensor parameters and failure events

2️⃣ Data Preparation

Removed identifier columns

Encoded categorical variables

Split dataset into training and testing sets

Prepared features and target variables

3️⃣ Model Development

A Logistic Regression model was selected because it:

Provides interpretable results

Produces probability outputs

Performs well for classification tasks

4️⃣ Model Evaluation

Model performance was evaluated using:

Confusion Matrix

Precision

Recall

F1 Score

Accuracy

📈 Results
Model Performance:

Accuracy: ~99.9%

Very strong class separation

Highly confident probability predictions

Confusion Matrix (Default Threshold = 0.5)
[[1939    0]
 [   2   59]]

Interpretation:

Correctly identified 1939 healthy machine states

Correctly detected 59 machine failures

Missed 2 failure events

Produced zero false alarms

🎚 Threshold Analysis

Threshold values between 0.3 and 0.9 were tested to evaluate classification sensitivity.

Results showed no performance change across these thresholds. This indicates:

The model produces highly confident predictions

Predicted probabilities are strongly separated between failure and non-failure classes

Minimal probability overlap exists between the classes

🔍 Model Interpretation

Logistic regression coefficients were analyzed to determine the influence of each feature on failure probability.

Key insight:

Certain operating conditions such as torque, temperature, and tool wear significantly influence failure risk.

This allows engineers to understand not only when failures may occur, but also why they occur.

Business Value

This predictive maintenance system can support industrial operations by:

Reducing unexpected machine downtime

Lowering maintenance costs

Improving production planning

Increasing operational safety

Supporting data-driven maintenance scheduling

The model can be integrated into real-time monitoring systems to generate machine risk scores based on live sensor data.

🛠 Tools & Technologies

Python

Pandas

NumPy

Scikit-learn

Matplotlib

Seaborn

Jupyter Notebook

Future Improvements

Compare additional machine learning models (Random Forest, XGBoost)

Perform cross-validation

Implement cost-sensitive learning strategies

Deploy model as an API for real-time prediction

Integrate with live industrial sensor systems

📁 Project Structure
Predictive-Maintenance/
│
├── data/
├── notebooks/
│   └── predictive_maintenance.ipynb
├── README.md
└── requirements.txt

Author

Felix Jeremiah Cudjoe
M.Sc. Manufacturing Engineering – TU Dortmund
Mechanical Engineer | Data Science Enthusiast | Predictive Maintenance & Industrial AI
