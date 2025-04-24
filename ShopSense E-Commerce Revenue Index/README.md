## Project Title : ShopSense: E-Commerce Revenue Index.

**Technologies Used**: 

**Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn

**Languages**: Python.

**Project Overview**:The goal of this project is to develop a predictive model for ShopSense's E-Commerce Revenue Index using historical order and transaction data. By analyzing key sales metrics, we aim to identify trends, forecast revenue, and optimize decision-making for online retail performance.

The model is trained on data up to 2022 Q3 and tested on 2022 Q4, evaluating multiple machine learning models to determine the most accurate revenue predictor. This project provides insights into the factors driving e-commerce revenue, helping businesses make data-driven strategic decisions.

**The project follows several steps:**

**1. Data Loading:** Loaded the dataset and inspected its structure.

**2.Data Exploration:** 
- Displayed basic statistics and sample rows to understand the structure.
- Identified missing values and inconsistencies.

**3.Data Preprocessing & Feature Engineering:** 

**Cleaning Order Numbers**
- Removed inconsistencies where order numbers were out of sequence.
- Calculated total_orders per quarter based on order number differences.
  
**Handling Outliers & Normalization**
- Removed outliers using the Interquartile Range (IQR) method.
- Normalized total_spend_index by dividing it by weekly_active_users_index to adjust for variations in user activity.
  
**Quarterly Aggregation**
- Converted daily data into quarterly summaries to match the revenue reporting period.

**4. Merging Data**: Combined order_numbers, transaction_data, and reported_data to create a consolidated dataset.

**5. Exploratory Data Analysis**: Understanding Revenue Trends over time from Merged Data.

**Observations** 
- Overall Growth: Revenue index shows an increasing trend from 2018 to 2022.
- Seasonal Fluctuations: Recurring spikes and dips suggest seasonal trends.
- Strong Growth in 2021-2022: Revenue peaked significantly during this period.
- Volatility: Some quarters show sudden declines after peaks, indicating variability.

**6. Model Training and Evaluation**
- **Models Tested:** Trained multiple models like Linear Regression, Decision Tree, and Random Forest.
- **Model Evaluation:** Evaluated models using metrics like Mean Absolute Error (MAE), Mean Squared Error (MSE) and Percentage error.

**7. Conclusion**: Random Forest Regressor model predicted well for 2022 Q4 Revenue Index after evaluating several models.
