# 📘 Stock Price Movement Prediction Using KNN
This project demonstrates how to use K-Nearest Neighbors (KNN) for both classification and regression to predict stock price movements based on historical price patterns. The dataset used is for Tata Consumer Products Ltd., retrieved from Yahoo Finance, and features were engineered to capture meaningful patterns from price volatility and changes.

#### 🧠 Project Objective
The goal is to:
- Classify whether a stock should be bought or sold the next day.
- Predict the actual closing price using KNN Regression.
- This is achieved by leveraging engineered features that capture the momentum and volatility of the stock prices.

#### 📊 Dataset
- The data is sourced from Yahoo Finance using the yfinance API for the ticker:
   - TATACONSUM.NS
##### Time Period:
   - Start Date: 2024-07-01  
   - End Date:   2025-07-01
#### 📌 Features Used
- Two features were engineered to form the input variables:
  -  Open - Close: Difference between opening and closing prices.
  -  High - Low: Intraday price range.

#### 🎯 Target Variables
- Classification Task:
- Target variable Y is assigned:
   - +1 for a Buy signal (if the next day's closing price is higher)
   - -1 for a Sell signal
- Regression Task:
   - Predict the actual closing price using regression.

#### 🛠️ Tools & Libraries
- Data Handling: pandas, numpy
- Visualization: matplotlib, seaborn
- Finance API: yfinance
- Machine Learning: scikit-learn
   -  KNeighborsClassifier, KNeighborsRegressor
   -  GridSearchCV for hyperparameter tuning
   -  train_test_split, accuracy_score

#### 🔍 Methodology
- 🔹 Classification using KNN
   - Feature Engineering on raw stock data.
   - Split into train/test sets (70/30).
   - Use GridSearchCV to find the optimal value of k (number of neighbors).
   - Train a KNeighborsClassifier.
   - Evaluate using Accuracy Score.

- 🔹 Regression using KNN
   - Target: Next day's closing price.
   - Train a KNeighborsRegressor.
   - Evaluate with suitable regression metrics (e.g., RMSE).

#### 📈 Sample Visualization
- Closing Price Line Plot
- Buy/Sell signals plotted
- Accuracy scores displayed for both training and testing data
