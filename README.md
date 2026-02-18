📊 Predicting Diabetes Progression: A Regularized ML Approach
This repository contains a comprehensive Machine Learning analysis focused on predicting the progression of diabetes one year after baseline using clinical and physiological data.

🎯 Project Objective
The goal of this project is to develop a robust regression model to forecast disease progression. 
The analysis emphasizes feature reliability, handling multicollinearity, and model interpretability, ensuring the results are not just statistically significant but also clinically relevant.

🗂️ Dataset Overview
We utilized the Scikit-Learn Diabetes Dataset, which consists of:

Patients: 442

Features: 10 physiological variables (Age, Sex, BMI, Blood Pressure, and 6 Blood Serum measurements).

Target: A quantitative measure of disease progression one year after baseline.

🛠️ Technical Workflow
The project follows a rigorous Data Science pipeline:

Exploratory Data Analysis (EDA): Visualizing distributions and identifying statistical properties of the target.

Feature Diagnostics: Using VIF (Variance Inflation Factor) and Mutual Information to detect high multicollinearity (especially in blood serum markers).

Baseline Modeling: Establishing an initial benchmark using simple Linear Regression.

Regularization Strategy: Implementing Ridge Regression (L2) to stabilize coefficients in the presence of redundant features.

Optimization: Hyperparameter tuning via Grid Search with Repeated K-Fold Cross-Validation (10-split, 3-repeat).

Residual Diagnostics: Conducting Breusch-Pagan tests for heteroscedasticity and Q-Q Plots for normality.

📈 Key Results
Generalization: Successfully achieved an R^2 approx 0.49 on the test set, with a minimal 2% gap from the training performance, indicating zero overfitting.

Precision: The model shows increased accuracy for high-risk patients (Target > 150), making it a valuable tool for clinical screening.

Insights: BMI and Serum Marker s5 were identified as the primary drivers of disease progression.

🚀 Future Improvements
Implementation of non-linear transformations (Polynomial Features).

Comparative analysis with Tree-based Ensemble models (XGBoost, Random Forest).

Advanced Feature Engineering to address residual heteroscedasticity.

💻 Technologies Used
Python (Pandas, NumPy)

Scikit-Learn (Modeling, Pipeline, CV)

Matplotlib & Seaborn (Visualization)

Statsmodels (Statistical Testing)
