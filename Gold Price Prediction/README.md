**Project Title : Gold Price Prediction.**

**Technologies Used:** Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, statsmodels, --- Languages: Python.

**Project Overview:** To build a machine learning model that accurately predicts gold prices (GLD) using key financial indicators like stock indices, oil prices, and currency exchange rates.

**Table of contents**
1. Dataset Loading
2. Data Exploration
3. Data Preprocessing
4. Exploratory Data Analysis (EDA)
5. Modelling
6. Time Series Analysis
7. Evaluation Metrics
8. Conclusion

**The project follows a structured pipeline as outlined below:**

  **1. Data Loading:** Load the dataset and inspect its structure.

  **2. Data Exploration:** Understand the dataset by checking distributions, missing values, duplicates, datatypes and key statistics.

**3. Data Preprocessing:** - Date converted to Date format

**4. Exploratory Data Analysis (EDA):** performed univariant and bivariant analysis.

- **Observations in univariant analysis** 

The distribution plots show a variety of shapes across the different financial indicators. SPX (S&P 500) appears right-skewed with multiple peaks, suggesting different market cycles over time. GLD (Gold prices) is fairly normally distributed but with a slight skew, indicating a consistent trading range. USO (oil prices) and SLV (silver prices) both show noticeable right-skewness and bimodal patterns, hinting at historical shocks or volatility in the commodities market. EUR/USD shows a clear bimodal distribution, which could reflect changing monetary policies or economic conditions across time.

- **Observations in Bivariant analysis**

In the correlation matrix, GLD and SLV are strongly linked, moving together. SPX has little correlation with gold but is negatively related to oil and the EUR/USD rate. USO and EUR/USD are positively correlated, likely due to global economic factors.

**5. Modeling: Applied machine learning models:**
Linear Regression, Random Forest Regressor.

**6. Time Series Analysis**

In addition to predicting gold prices using machine learning models, time series analysis was applied to forecast future trends. The following steps were followed:

- **Understanding Trends and Seasonality** : Visualized the overall trend and seasonal variations in gold prices.
  
  **Observations**:

  - Gold prices show a general upward trend over time, but with clear fluctuations. There may be some seasonality to these price swings. A sharper price increase is apparent in the more recent data.

  - This time series decomposition shows clear and regular patterns. The original series has a repeating upward pattern, indicating strong cyclic behavior over the years. The trend component steadily increases in steps, suggesting periodic resets or cycles in the overall level. The seasonality is consistent throughout the time span, showing a repeating short-term pattern, likely monthly or quarterly. The residuals reveal sharp spikes at regular intervals, meaning some events aren't fully explained by trend or seasonality—possibly anomalies or outliers.


- **Stationarity Check**
  
Performed the Augmented Dickey-Fuller (ADF) test to check whether the data is stationary or not. Here, data is not stationary. So it is necessary to eliminate trends by using differencing techniques to make the data stationary.

- **Building Time Series Models**
  
ARIMA: Auto-Regressive Integrated Moving Average model.

SARIMA: Seasonal ARIMA model to handle seasonality in the data.

**7. Evaluation**
  
The models were evaluated based on Mean Squared Error (MSE) and R2_Score to determine their forecasting accuracy.

**8. Conclusion:** 

- The Random Forest Regressor model, performed well in predicting gold prices, showing a strong correlation between the selected financial features and gold value. This demonstrates the potential of machine learning in financial forecasting and investment decision support.

