# 🎬 Movies Success Prediction using Machine Learning

This project aims to analyze and predict movie success using 
machine learning models based on various features like budget, 
runtime, language, genres, and more. It uses both regression 
techniques (for predicting revenue and ROI) and exploratory 
data analysis to extract insights from the dataset.

---

## 📌 Project Author

**Muhammad Arslan ul Haq**

---

## 📁 Project Overview

This Jupyter Notebook walks through a complete machine learning pipeline to:

- Clean and prepare movie data
- Perform exploratory data analysis (EDA)
- Engineer relevant features
- Predict movie **revenue** and **Return on Investment (ROI)** using:
  - Random Forest Regressor
  - Gradient Boosting Regressor
  - Linear Regression
- Evaluate model performance with metrics such as:
  - R² Score
  - RMSE (Root Mean Squared Error)
  - MAE (Mean Absolute Error)
- Visualize:
  - Model performance
  - Actual vs Predicted values
  - Feature importances

---

## 📊 Dataset

The dataset contains information about movies including:
- Title
- Budget
- Revenue
- Runtime
- Release Year and Month
- Genre
- Language
- ROI (calculated as `revenue / budget`)

> 📌 ROI categories were created for classification insight:
> - Flop
> - Break-even
> - Success
> - Blockbuster

---

## ⚙️ Machine Learning Models

The following models were implemented and evaluated:

- **Random Forest Regressor**
- **Gradient Boosting Regressor**
- **Linear Regression**

Each model was trained and tested on:
- **Revenue prediction**
- **ROI prediction**

### 🔍 Best Performing Model:
- **Revenue**: Random Forest (highest R² score)
- **ROI**: Gradient Boosting

---

## 🧠 Key Features Used

- `budget_log` (log-transformed budget)
- `runtime`
- `release_month`
- `language_encoded` (LabelEncoded language)
- `decade` (based on release year)
- `vote_count`
- One-hot encoded top genres:
  - Drama, Comedy, Action, Thriller, Romance, Adventure, Crime, Science Fiction

---

## 📈 Visualizations

The notebook includes rich visual output including:

- Model performance comparison (R² scores)
- Top 10 important features (Random Forest)
- Actual vs Predicted scatter plot
- ROI prediction comparison

---

## 📦 Dependencies

Install the following Python libraries:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn
