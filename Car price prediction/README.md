**Project Title : Car Price Prediction using Machine Learning.**

**Technologies Used:** Libraries: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn --- Languages: Python.

**Project Overview:** The aim of this project is to predict car prices based on the car name, type of the fuel, Kms_Driven and year.

**Table of contents**
1. Dataset Loading
2. Data Exploration
3. Exploratory Data Analysis (EDA)
4. Modelling
5. Evaluation Metrics
6. Conclusion

**The project follows a structured pipeline as outlined below:**

  **1. Data Loading:** Load the dataset and inspect its structure.

  **2. Data Exploration:** Understand the dataset by checking distributions, missing values, datatypes and key statistics.

**3. Exploratory Data Analysis (EDA):** performed univariant and bivariant analysis.

- **Observations in univariant analysis** 

- Most cars use Petrol, with far fewer Diesel and very few CNG. Dealers have listed more cars than individuals. Manual transmission dominates over automatic, and nearly all cars are first-hand.

- The most frequently listed car in the dataset is the Maruti City, appearing 26 times, followed by models like the Corolla Altis (16), Verna (14), and Fortuner (11).

- Cars are mostly from 2010–2017, showing a focus on relatively new vehicles. Selling and present prices are right-skewed, with most cars priced low and a few high-end ones. Kms_driven also has a long tail, with some high-mileage outliers.

- **Observations in Bivariant analysis**

- Present price has a strong positive correlation with selling price, and newer cars tend to sell for more. Kms driven has almost no effect on selling price but is negatively correlated with the car’s year, meaning older cars are driven more.

**4. Modeling:** 

**Applied various machine learning models:**
Linear Regression, RandomForestRegressor, Lasso Regression.

**5. Evaluation**
  
The models were evaluated based on Mean Absolute Error (MAE) and R2 Score to determine their accuracy.

**6. Conclusion:** 

- The Random Forest model provided the most accurate predictions for Car prices, with an R² score of 0.96.


