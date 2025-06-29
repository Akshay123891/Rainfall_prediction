# 🌧️ Rainfall Prediction Project (Austin Weather Data)

This project aims to predict **precipitation levels** using **Linear Regression** on historical weather data from **Austin, Texas**. It is part of **Module 13 - Assignment 6** in the Data Science course.

---

## 📁 Dataset

- **austin_weather.csv**: Contains daily weather parameters such as:
  - Average Temperature
  - Humidity
  - Wind Speed
  - Dew Point
  - Visibility
  - Precipitation

> Dataset source: Provided in the LMS (Module 12 > Project - COVID-19 Analysis > Case Study - Part 1 > Resource 1)

---

## 🧠 Objective

To predict the `PrecipitationSumInches` (amount of daily rainfall) based on other weather features using **Linear Regression**, and to:
- Clean and preprocess the data.
- Handle missing and irregular values like `"T"` (trace) and `"-"`.
- Analyze feature relationships using visualizations.
- Evaluate model accuracy and interpret regression results.

---

## 🛠️ Tools & Libraries Used

- Python
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn (Linear Regression)

---

## 📊 Project Workflow

### 1. Data Loading
- Load `austin_weather.csv` using `pandas`.

### 2. Data Cleaning
- Drop non-numeric columns like `Date`, `Events`.
- Replace symbols `'T'` and `'-'` with `0`.
- Convert data to float and drop missing values.

### 3. Feature Selection
- Input features: temperature, humidity, dew point, wind speed, etc.
- Target variable: `PrecipitationSumInches`.

### 4. Model Training
- Split dataset using `train_test_split()`.
- Fit a **LinearRegression** model on training data.

### 5. Evaluation
- Mean Squared Error (MSE)
- R-squared Score (R²)
- Regression Coefficients

### 6. Visualizations
- Heatmap of correlations
- Precipitation trend line
- Scatter plots:
  - Humidity vs Precipitation
  - Wind Speed vs Precipitation

---

## 📈 Sample Results

```txt
Mean Squared Error (MSE): 0.135
R-squared Score (R²): 0.48

Feature Coefficients:
TemperatureAvgF            0.012
HumidityAvgPercent         0.045
WindSpeedAvgMPH           -0.010
...
REQUIREMENTS:
pip install pandas numpy matplotlib seaborn scikit-learn
