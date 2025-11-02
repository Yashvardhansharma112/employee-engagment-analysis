🚀 HR Analytics Project: Employee Attrition Analysis & Prediction

Project Goal

This project addresses the critical business challenge of employee turnover by analyzing historical HR data to uncover the root causes of attrition and predict which employees are most likely to leave. The primary deliverables are a complete analysis pipeline and an interactive data visualization dashboard built with Streamlit.

💡 Key Business Insights & Deliverables

Identified Top Drivers of Attrition: Determined the most statistically significant factors contributing to employee churn (e.g., Overtime, Monthly Income, Years at Company) through Exploratory Data Analysis (EDA) and Feature Importance analysis.

Predictive Model: Built and evaluated a Random Forest Classifier to flag at-risk employees, achieving strong performance metrics (details available in the model metrics section of the dashboard).

Interactive Dashboard: Developed a Streamlit application to visualize overall and filtered attrition rates, key distribution plots, and the model's performance metrics for HR decision-makers.

🛠️ Technology Stack

Category

Tools

Purpose

Data Processing

Python, Pandas, NumPy

Data manipulation, cleaning, and feature engineering.

Statistical Modeling

Scikit-learn

Building and evaluating the Random Forest Classification model.

Visualization & App

Streamlit, Seaborn, Matplotlib

Creating the interactive dashboard and complex statistical plots.

Data Source

WA_Fn-UseC_-HR-Employee-Attrition.csv

Fictional but realistic IBM HR Analytics dataset.

⚙️ Project Workflow (Pipeline)

Data Loading & Cleaning: Loaded the dataset and handled missing values, duplicates (none found), and dropped constant/irrelevant columns (EmployeeCount, StandardHours, Over18).

Exploratory Data Analysis (EDA): Calculated base attrition rates and used visual comparisons (countplot, boxplot) to examine the relationship between categorical features (Department, OverTime) and numerical distributions (MonthlyIncome, YearsAtCompany) against the target variable (Attrition).

Data Preprocessing: Prepared features for the model by encoding all categorical variables using One-Hot Encoding and splitting the data into training and testing sets.

Predictive Modeling: Trained a Random Forest Classifier (using balanced class weights to account for class imbalance) to predict attrition.

Model Evaluation & Feature Importance: Assessed model performance using a confusion matrix, classification report (Precision, Recall), and extracted the top 10 most influential factors for prediction.

Interactive Dashboard: Deployed the analysis and model results into an interactive Streamlit application (app.py) for easy stakeholder consumption.

🎯 Actionable Recommendations

Based on the EDA and the feature importance analysis, the following are the most critical strategies to improve employee retention:

Target Overtime: Overtime is consistently ranked as a top predictor of attrition. Implement strict workload management policies and consider offering compensatory time off, especially in high-churn operational roles.

Address Income Gaps: The median income for employees who left is statistically lower. Conduct a compensation and market parity review for lower Job Levels and roles like Sales Representative to ensure competitive financial incentives.

Invest in Early Career Retention: Attrition rates are highest for employees with low Total Working Years and Years at Company. Develop robust, mandatory mentorship programs focused on the first 1-3 years of tenure to improve job involvement and long-term commitment.

Boost Non-Monetary Factors: Prioritize programs that enhance Job Satisfaction and Environment Satisfaction, as these non-monetary ratings are critical retention factors highlighted by the model.

💻 How to Run the Dashboard Locally

To reproduce the full analysis and run the interactive dashboard, follow these steps:

Requirements

You will need Python and the following libraries installed:

pip install pandas numpy scikit-learn matplotlib seaborn streamlit


Execution

Ensure the dataset (WA_Fn-UseC_-HR-Employee-Attrition.csv) and the application file (app.py) are in the same folder.

Open your terminal or command prompt in that directory.

Run the Streamlit application:

streamlit run app.py


The application will automatically open in your default web browser, allowing you to interact with the filters and explore the insights.
