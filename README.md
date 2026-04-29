
# ⚽ Football Player Market Value Prediction

This project is a data analysis and machine learning study developed for the market value estimation. It implements a **Random Forest Regressor** model to predict the market values of football players based on their physical attributes, career statistics, and performance data.

## 📝 Project Overview
The study utilizes the "Transfermarkt" database sourced from Kaggle. Multiple relational datasets, including match performances (~1.2M+ rows in `appearances.csv`), player profiles (~30,000+ rows in `players.csv`), and current market values (`player_valuations.csv`), were integrated into a clean, feature-rich pipeline using SQL-like JOIN operations.

The model learns to estimate financial values by analyzing key features. During the process, target normalization (log-transformation) was applied to stabilize the variance in the highly skewed football market.

## 📊 Model Performance
* **Algorithm:** Random Forest Regressor
* **R-squared (R²):** 0.49
* **Mean Absolute Error (MAE):** €2.6M

*(Note: The model identifies "Minutes Played" and "Age" as the most significant drivers of market value. While highly accurate for the majority of professional players, the model is naturally conservative with "Superstar" outliers (over €100M) due to the lack of intangible data such as brand value and contractual release clauses.)*

## 📂 Repository Contents
* 📓 `MarketValue.ipynb`: Detailed Jupyter Notebook containing data cleaning, feature engineering, and the training phases of the Random Forest model.
* 📊 `Random-Forest-Regressor-Predicting-Football-Player-MarketValues.pdf`: A comprehensive presentation explaining the mechanics of the Random Forest algorithm (Bagging, Bootstrap Aggregation) and the Pros/Cons of the model.

## 🚀 Technologies Used
* **Language:** Python
* **Data Manipulation:** Pandas, NumPy
* **Machine Learning:** Scikit-learn
* **Data Visualization:** Matplotlib, Seaborn
