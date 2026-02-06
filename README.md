### Project Title: HR Analytics - Predicting Employee Attrition
Objective:
To build a machine learning solution that predicts which employees are likely to leave the company and identifies the root causes of turnover to help the HR department improve retention.

### Tech Stack:
Python: Pandas, Seaborn (EDA), Scikit-Learn (Modeling), SHAP (Explainability).
Power BI: Interactive Dashboard for business insights.
Data: IBM HR Analytics Employee Attrition Dataset.
Key Activities & Workflow:

### Data Preprocessing:
- Performed Exploratory Data Analysis (EDA) to examine distributions of age, income, and job roles.
- Handled categorical data using One-Hot Encoding and Label Encoding.
- Removed noise (irrelevant columns like EmployeeCount, StandardHours).

### Machine Learning Modeling:
- Built a Decision Tree Classifier to predict attrition.
- Addressed class imbalance (few people quitting vs. many staying) by applying class_weight='balanced', improving the model's ability to detect potential leavers (Recall score improved to 41%).
- Achieved a final Model Accuracy of 77%.

### Model Explainability (SHAP):
- Integrated SHAP (SHapley Additive exPlanations) to interpret the "Black Box" model.
- Identified that OverTime, Monthly Income, and Job Level are the top three drivers of employee attrition.

### Business Intelligence (Power BI):
- Developed an interactive dashboard visualizing Attrition Rate (16.1%) and demographic breakdowns.
- Created visualizations to highlight the correlation between OverTime and turnover.

### Key Insights:
- Employees working OverTime are significantly more likely to quit.
- Junior Employees (Job Level 1) and those with Low Stock Options have the highest churn rate.
