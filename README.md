# Goldman Sachs — Loan Portfolio Analysis & Default Prediction

## Project Overview

This capstone project analyzes loan portfolio data to identify repayment patterns, explore potential default risks, and generate actionable business insights using **SQL, Power BI, and Python**.

The project combines data analysis, interactive visualization, and machine learning to support data-driven loan risk assessment and portfolio monitoring.

## Objectives

- Analyze loan status distribution and customer patterns using SQL.
- Visualize portfolio composition and repayment indicators using Power BI.
- Develop a machine learning model to identify loans associated with charge-off outcomes.
- Examine feature associations and evaluate model performance.
- Provide practical recommendations for risk monitoring and portfolio health.

## Tools & Technologies

- **SQL:** Data querying, joins, aggregations, and business analysis.
- **Power BI:** Interactive dashboards and data visualization.
- **Python:** Data preparation, feature engineering, and machine learning.
- **Pandas:** Data manipulation and analysis.
- **Scikit-learn:** Preprocessing, Logistic Regression, and model evaluation.
- **Matplotlib:** Feature importance visualization.
- **Jupyter Notebook:** Model development and documentation.

## Project Workflow

### 1. SQL Analysis

- Examined loan status distribution.
- Analyzed customer distribution across regions.
- Summarized historical loan information to identify patterns for further investigation.

### 2. Power BI Dashboard

- Visualized loan portfolio composition and repayment indicators.
- Supported comparisons across available loan and customer categories.
- Presented portfolio information in an interactive format for business review.

### 3. Python — Loan Default Prediction

A Logistic Regression model was trained to classify historical loans as **Fully Paid** or **Charged Off**.

The modeling dataset contained **94,212 records**:

- Fully Paid: 76,361
- Charged Off: 17,851

Data preprocessing included missing-value handling, categorical encoding, numerical scaling, and a stratified train-test split.

### Model Evaluation

| Metric | Result |
|---|---:|
| Accuracy | 63.55% |
| Precision | 28.19% |
| Recall | 59.72% |
| F1-score | 38.30% |

The model identified approximately 59.72% of charged-off loans in the test dataset. Its precision of 28.19% indicates that many loans flagged as charged off were actually fully paid. Therefore, the model is better suited to preliminary risk screening than to making automatic lending decisions.

## Key Business Insights

- Current loans represent the largest category in the loan dataset, making ongoing portfolio monitoring important.
- Regional customer counts describe customer distribution but do not independently establish regional default risk.
- Loan purpose, state, and home ownership showed associations with model predictions; these relationships are not evidence of causation.
- Model predictions should be combined with verified financial information and human review.
- Consistent KPI definitions across SQL and Power BI are essential for reliable reporting.

## Recommendations

- Monitor active loans separately from loans with final repayment outcomes.
- Compare default rates across loan segments using clearly defined denominators.
- Review high-risk predictions rather than automatically rejecting customers.
- Evaluate false positives, missed defaults, and model performance regularly.
- Improve data quality and collect genuine application decision records for future approval-model development.

## Data Limitations

The available dataset contains repayment outcomes rather than genuine loan application decisions. Consequently, a reliable approval prediction model could not be trained using the available data alone.

The dataset also does not contain a genuine credit-score field. The default model predicts historical **Fully Paid versus Charged Off** outcomes and should not be interpreted as a loan approval model.

## Conclusion

This project demonstrates the application of SQL, Power BI, and Python to loan portfolio analysis and default-risk investigation. It combines descriptive analysis, interactive visualization, and machine learning to identify patterns and support business recommendations.

The results highlight the value of data-driven risk monitoring while emphasizing the importance of model limitations, reliable data, and human judgment in lending decisions.

## Author

**Sonaal Thakur**  
Data Analytics Capstone Project

**Skills demonstrated:** SQL • Power BI • Python • Data Analysis • Machine Learning • Data Visualization • Business Insights
