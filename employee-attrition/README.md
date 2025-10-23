🧠 Employee Attrition Prediction using Machine Learning
🎯 Project Overview

This project uses machine learning to predict employee attrition — whether an employee will leave the company — based on a dataset of HR factors. The goal is to identify key drivers of attrition so the HR department can implement targeted retention strategies.

Dataset: IBM HR Analytics Employee Attrition Dataset (Kaggle)

🛠️ Technology Stack

Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

Tools: Jupyter Notebook / VS Code

📊 Key Findings & Feature Importance

The analysis identified the following factors as the most predictive of attrition:

OverTime: Employees working overtime are significantly more likely to leave.

MonthlyIncome: Lower monthly income correlates strongly with higher attrition risk.

JobSatisfaction: Lower satisfaction levels are a major predictor of leaving.

YearsAtCompany: Employees with fewer years at the company (often recent hires) show higher turnover.

📈 Model Performance

A comparison of several classification models was performed. Random Forest provided the best balance of performance, achieving a high Recall for the 'Yes' (Attrition) class, which is critical for minimizing false negatives (employees at risk that we fail to identify).

Model	Accuracy	Precision (Yes)	Recall (Yes)	F1-Score (Yes)
Random Forest	0.8673	0.8000	0.5517	0.6521
Logistic Regression	0.7789	0.4444	0.7931	0.5701
Decision Tree	0.8163	0.5000	0.6207	0.5540

Note: The models were trained with class_weight='balanced' to better handle the imbalanced dataset.

💡 Recommendations for HR

Based on model insights, the following recommendations are provided to improve employee retention:

Overtime Policy Review: Implement stricter controls or compensatory policies (e.g., compressed work weeks, time-off) for employees consistently working overtime.

Compensation Benchmarking: Review salary bands, especially for high-risk roles/departments, to ensure monthly income is competitive.

Engagement & Satisfaction: Introduce mandatory quarterly, anonymous job satisfaction surveys, with management required to present action plans for low-scoring teams.

Onboarding & Mentorship: Focus retention efforts on employees during their first 2–3 years at the company through mentorship programs and career path planning.