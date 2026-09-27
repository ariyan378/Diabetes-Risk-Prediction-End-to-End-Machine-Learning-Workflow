<div align="center">
  <!-- Animated Logo / Graphic -->
  <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExM2QzZGNjMzJmZGZiMzJkM2M3YzUzYmQ3YmFkMjRiYjM1ZGVmNzViOCZlcD12MV9pbnRlcm5hbF9naWZzX2dpZklkJmN0PWc/3o7TKoWZlO3qqv08Qo/giphy.gif" alt="Animated Heartbeat Data" width="200"/>

  # 🩸 Diabetes Risk Prediction Pipeline

  **An End-to-End Machine Learning Workflow for Healthcare Data**

  [![Python](https://img.shields.io/badge/Python-3.8+-blue.svg?style=for-the-badge&logo=python&logoColor=white)]()
  [![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458.svg?style=for-the-badge&logo=pandas&logoColor=white)]()
  [![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-Machine%20Learning-F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)]()
</div>

---

## 📖 Project Overview

This project provides a complete machine learning workflow to predict a person's risk of diabetes[cite: 1]. The system uses health and lifestyle data to classify patients into three risk categories: Low, Moderate, and High[cite: 1]. 

The main goal is to show a clean, step-by-step process for data cleaning, visualization, and model training[cite: 1]. This project was built for the NLP & ML Research Lab at Daffodil International University[cite: 1].

## 📊 Dataset Details

The model learns from the `diabetes_risk.csv` dataset, which contains 15,000 patient records and 19 different columns[cite: 1]. 

The data includes lifestyle habits, like diet and sleep, along with strict medical measurements[cite: 1]. The target we want to predict is `diabetes_risk`, which is imbalanced because 60% of the patients are in the Low-risk group[cite: 1]. 

## ⚙️ Machine Learning Workflow

The project follows a standard data science pipeline to prepare the data and train the models[cite: 1]:

* **Data Cleaning:** We removed empty values by filling them with the most common answers and handled extreme medical numbers by capping them instead of deleting the rows[cite: 1].
* **Feature Engineering:** We created new helpful data points, like combining blood pressure readings into a single "Mean Arterial Pressure" score and grouping BMI into standard medical bands[cite: 1].
* **Feature Selection:** We used a Random Forest tool to find the top 15 most important data points, dropping weak features like city names to reduce noise[cite: 1].
* **Model Training:** We trained three separate models: Logistic Regression, Random Forest, and Gradient Boosting[cite: 1].

## 🏆 Key Findings & Results

The tree-based models (Random Forest and Gradient Boosting) performed the best because they can handle complex, non-linear health patterns better than simple linear models[cite: 1]. 

The most important factors for predicting diabetes risk are HbA1c levels, fasting blood sugar, BMI, age, and waist size[cite: 1]. Lifestyle answers (like city or diet) provided very little predictive value compared to the actual medical tests[cite: 1].

## 🚀 Action Items: How to Run This Project

Follow these steps to set up the project on your local machine:

* Clone this repository to your local computer using your terminal.
* Install the required Python libraries (Pandas, NumPy, Matplotlib, Seaborn, and Scikit-Learn)[cite: 1].
* Place the `diabetes_risk.csv` dataset in the main project folder[cite: 1].
* Open the Jupyter Notebook file in your code editor.
* Run the code cells one by one from top to bottom.
* Check the output plots to see the data relationships and final model scores.
