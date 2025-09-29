# 📊 Data Mining on Yelp Dataset

This project focuses on **exploring, analyzing, and building data science solutions using the Yelp Dataset**. The analysis is divided into two major parts:

1. **Exploratory Data Analysis (EDA)** — Understanding business distributions, popular categories, ratings, and trends.  
2. **Data Science Problems** — Implementing predictive and recommendation models to solve real-world business and user problems.

---

## 🧠 Problem Statement

The project addresses two key problems using Yelp data:

- **Problem 1: Check-in Popularity Prediction**  
  Predict whether a business is *popular* or *not* based on its historical check-in patterns.

- **Problem 2: Location-Based Recommendation System**  
  Recommend top locations to entrepreneurs for opening new restaurants and to users for finding the best nearby restaurants.

---

## 📂 Dataset Used

- **Yelp Business Data** – Contains details like name, categories, city, stars, review count, latitude, and longitude.  
- **Yelp Check-in Data** – Includes aggregated check-in information by hour-day combinations.  

---

## 🧪 Exploratory Data Analysis

- Distribution of business star ratings  
- Top 10 business categories and cities  
- Top-rated businesses  
- Restaurant counts by city  
- Top restaurant subcategories

These analyses help identify trends in business types, city distributions, and customer preferences.

---

## 📈 Data Science Problem 1: Check-in Popularity Prediction

### 📝 Objective
Classify businesses as **popular (1)** or **not popular (0)** based on their check-in behavior.

### ⚙️ Methodology
- Feature engineering from check-in patterns:
  - Active time slots
  - Morning/afternoon/evening/late ratios
  - Weekday vs weekend activity
- Train/test split
- Model training:
  - Logistic Regression
  - Decision Tree Classifier
  - Random Forest Classifier

### 📊 Model Comparison (Train vs Test)
A line plot was used to visualize train vs test accuracy across models, highlighting potential overfitting.

| Model          | Train Accuracy | Test Accuracy |
|---------------|---------------|---------------|
| LogReg        | ~0.964        | ~0.963        |
| DecisionTree  | ~0.999        | ~0.972        |
| RandomForest  | ~0.999        | ~0.977        |

---

## 📍 Data Science Problem 2: Location-Based Recommendation System

### 🏢 For Entrepreneurs
Identify the **best cities, ZIP/postal codes, and geo-hotspots** to open new restaurants using:
- Average ratings
- Log-transformed review counts
- Success ratio (restaurants with high stars & sufficient reviews)
- KMeans clustering on latitude-longitude for hotspot detection

### 👤 For Users
Recommend **top nearby restaurants** within a given radius using latitude & longitude inputs.

---

## 🛠️ Tech Stack

- **Language:** Python 3  
- **Libraries:**  
  - `pandas`, `numpy` – Data manipulation  
  - `matplotlib` – Visualization  
  - `scikit-learn` – ML models and evaluation  
  - `KMeans` – Clustering for hotspot detection

---

