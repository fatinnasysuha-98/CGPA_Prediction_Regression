# 🎓 Student CGPA Prediction Using Mental Health & Academic Factors

## 📌 Overview

This project aims to predict students' **CGPA (Cumulative Grade Point Average)** using factors related to mental health, academic engagement, lifestyle habits, and study behavior.

The project follows a complete data analytics and machine learning workflow, including data loading, exploratory data analysis (EDA), data cleaning, feature engineering, data transformation, and regression model evaluation.

The objective is to identify which factors have the strongest influence on academic performance and build predictive models that can estimate students' CGPA accurately.

---

## 📂 Dataset

The dataset contains **1,000 student records** with information related to:

* Demographics (Gender, Age, Year of Study)
* Mental health indicators

  * Depression
  * Anxiety
  * Panic Attacks
  * Mental Health Support
* Lifestyle habits

  * Sleep Quality
  * Study Stress Level
  * Study Hours per Week
* Academic Engagement
* CGPA (Target Variable)

### Dataset Size

* Rows: 1,000
* Columns: 16 (before cleaning)

---

## 🛠 Tools & Technologies

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-Learn
* XGBoost

### Machine Learning Models

* Linear Regression
* Random Forest Regressor
* XGBoost Regressor
* Support Vector Regressor (SVR)
* K-Nearest Neighbors (KNN)
* Multi-Layer Perceptron (MLP) Regressor

---

## 🔍 Exploratory Data Analysis (EDA)

The dataset was explored to understand its structure and identify patterns.

### Analysis Performed

* Dataset inspection
* Data type validation
* Summary statistics
* Unique value analysis
* Feature distributions
* Correlation analysis
* Correlation heatmap
* Pairplot visualization
* Feature importance analysis
* Outlier detection using:

  * Boxplots
  * Interquartile Range (IQR)

### Key Insights

* Study Hours Per Week showed the strongest positive relationship with CGPA.
* Academic Engagement was positively associated with academic performance.
* Mental health-related variables showed weaker correlations with CGPA.
* The CGPA distribution was relatively balanced with no significant skewness.

---

## 🧹 Data Cleaning & Preparation

Several preprocessing steps were performed to prepare the data for modeling.

### Cleaning Steps

#### 1. Missing Value Check

* Verified that no missing values existed in the dataset.

#### 2. Duplicate Records Check

* No duplicate records were found.

#### 3. Feature Selection

Removed non-essential columns:

* Timestamp
* Course

#### 4. Categorical Encoding

Converted categorical features into numerical values:

* Gender → Label Encoding
* Year of Study → Numeric format

#### 5. Data Validation

* Verified all features were numeric.
* Reset dataset index after cleaning.

---

## ⚙️ Feature Engineering & Transformation

To improve model performance, several transformation techniques were explored:

### Standardization

* StandardScaler

### Normalization

* MinMaxScaler

### Log Transformation

* Log Scaling

These techniques were evaluated to determine their impact on model performance.

---

## 🤖 Machine Learning Models

The cleaned dataset was split into:

* Training Set: 70%
* Testing Set: 30%

Several regression algorithms were trained and evaluated.

### Models Tested

1. Linear Regression
2. Random Forest Regressor
3. XGBoost Regressor
4. Support Vector Regressor (SVR)
5. K-Nearest Neighbors (KNN)
6. Multi-Layer Perceptron (MLP) Regressor

---

## 📊 Model Evaluation

Models were evaluated using:

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

### Performance Summary

| Model                          | R² Score |
| ------------------------------ | -------- |
| Random Forest Regressor        | 0.9415   |
| Support Vector Regressor (SVR) | 0.9424   |
| XGBoost Regressor              | 0.9227   |
| K-Nearest Neighbors (KNN)      | 0.9255   |
| MLP Regressor                  | 0.9120   |
| Linear Regression              | 0.9065   |

### Best Performing Model

🏆 **Support Vector Regressor (SVR)** achieved the highest predictive performance with an R² score of approximately **94.2%**.

---

## 📈 Results

The analysis demonstrates that academic engagement and study habits play a significant role in predicting student CGPA.

Key findings include:

* Study Hours Per Week was the most influential predictor.
* Academic Engagement positively impacts academic performance.
* Mental health variables contribute to CGPA prediction but with lower influence compared to study-related factors.
* Machine learning models can accurately predict student academic outcomes using behavioral and mental health indicators.

---

## 🚀 Future Improvements

Potential enhancements for future work:

* Hyperparameter tuning for all models
* Cross-validation for improved robustness
* Feature selection optimization
* Advanced ensemble learning techniques
* Deployment using Streamlit or Flask
* Interactive dashboard development with Power BI
