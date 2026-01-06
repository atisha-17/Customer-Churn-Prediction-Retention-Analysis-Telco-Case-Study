# Customer-Churn-Prediction-Retention-Analysis-Telco-Case-Study
Customer churn is a critical business challenge for subscription-based companies.
This project focuses on identifying high-risk customers, understanding churn drivers, and translating predictive insights into actionable retention strategies.
The solution combines SQL, Python-based analytics, machine learning, NLP, and Power BI dashboards to deliver an end-to-end churn analysis pipeline designed for business stakeholders.

**Dataset**
Source: Enriched Telco Customer Churn Dataset (Kaggle)
Size: 7,043 customers × 23 features
Data Includes:
Demographics
Services & contract details
Billing information
Churn labels
AI-generated customer feedback (for sentiment analysis)

Tools & Technologies
SQL: SQLite (data ingestion & analysis)
Python: pandas, numpy, matplotlib, seaborn
Machine Learning: Logistic Regression, Random Forest
Deep Learning: LSTM (time-series modeling)
NLP: VADER Sentiment Analysis
Visualization: Power BI
Environment: Jupyter Notebook

Project Workflow
Cleaned and prepared the Telco churn dataset by fixing missing TotalCharges, standardizing data types, and converting churn labels into binary values.
Loaded the cleaned data into a SQLite database and used SQL to analyze churn patterns across contract types, payment methods, and services.
Performed EDA to understand customer behavior and identify churn-heavy segments such as month-to-month customers, fiber optic users, and new customers (≤3 months tenure).
Engineered churn-focused features including tenure in years, annualized charges, and customer lifecycle indicators to better capture behavioral risk.
Built a baseline Logistic Regression model and improved performance using Random Forest, achieving ROC-AUC scores up to ~0.79.
Implemented an LSTM model to experiment with tenure-based sequential patterns and time-aware churn behavior.
Applied VADER sentiment analysis on customer feedback and integrated sentiment scores into the modeling pipeline.
Generated customer-level churn probabilities and grouped customers into low, medium, and high-risk categories.
Designed a Power BI dashboard focused on decision-making rather than reporting, with executive KPIs, churn segmentation, risk distribution, high-risk customer views, and explainability through churn drivers.
Translated analytical findings into clear, actionable retention strategies for business stakeholders.

Key Insights
Month-to-month customers churn far more frequently than those on long-term contracts.
Customers with high monthly charges and fiber optic service show elevated churn risk.
Early-tenure customers are significantly more likely to churn.
Negative customer sentiment strongly aligns with higher churn probability.
