# ⚽ Football Injury Analytics & Prediction

An end-to-end Data Analytics and Machine Learning project that analyzes football player injury risk and predicts whether a player is likely to suffer an injury in the next season.

---

# 📑 Table of Contents

- [🎯 Project Mission](#-project-mission)
- [📌 About the Project](#-about-the-project)
- [🎯 Objectives](#-objectives)
- [📊 Dataset](#-dataset)
- [🧹 Data Cleaning](#-data-cleaning)
- [📈 Exploratory Data Analysis (EDA)](#-exploratory-data-analysis-eda)
- [📊 Power BI Dashboard](#-power-bi-dashboard)
- [🤖 Machine Learning](#-machine-learning)
- [📊 Model Performance](#-model-performance)
- [🌐 Deployment](#-deployment)
- [🛠️ Technologies Used](#️-technologies-used)

  
# 🎯 Project Mission

Football injuries can negatively affect both player performance and team success. Identifying players who are at higher risk of injury helps coaches, medical staff, and performance analysts make informed decisions regarding training load, recovery, and injury prevention.

The mission of this project is to combine data analytics and machine learning to identify the key factors associated with football injuries, visualize injury patterns through an interactive dashboard, and build a predictive model that estimates injury risk for the next season.

This project demonstrates a complete end-to-end analytics workflow, from raw data preprocessing to dashboard development, machine learning, and deployment.


# 📌 About the Project

Football injuries can significantly impact team performance and player careers. This project analyzes the factors associated with football injuries and builds a predictive machine learning model to estimate injury risk for the following season.

The project covers the complete data analytics workflow, including data cleaning, exploratory data analysis (EDA), dashboard development, machine learning, and deployment.

---

## 🎯 Objectives

- Analyze the main factors affecting football injuries.
- Discover relationships between player fitness and injury risk.
- Build an interactive Power BI dashboard.
- Train a Machine Learning model to predict future injuries.
- Deploy the trained model using Gradio.

---

## 📊 Dataset

The dataset contains information for **800 football players**.

### Features

- Age
- Height
- Weight
- BMI
- Position
- Training Hours per Week
- Matches Played (Previous Season)
- Previous Injury Count
- Knee Strength Score
- Hamstring Flexibility
- Reaction Time
- Balance Test Score
- Sprint Speed
- Agility Score
- Sleep Hours
- Stress Level
- Nutrition Quality
- Warm-up Routine Adherence

### Target

- **Injury Next Season**
    - 0 → No Injury
    - 1 → Injury

---

# 🧹 Data Cleaning

The following preprocessing steps were performed:

- ✔ No Missing Values
- ✔ No Duplicate Records
- ✔ Verified BMI calculation
- ✔ Converted Position into categorical values
- ✔ Created new categorical features:
  - Training Level
  - Sleep Category
  - Nutrition Category
  - Match Load
  - Injury History
- ✔ Outliers were retained because they represent realistic player performance rather than data entry errors.

---

# 📈 Exploratory Data Analysis (EDA

EDA was performed to understand player characteristics and identify factors associated with injury risk.

The analysis included:

- Distribution Analysis
- Correlation Analysis
- Injury Rate Analysis
- Position Analysis
- Match Load Analysis
- Sleep Analysis
- Stress Analysis
- Nutrition Analysis

---

# 📊 Power BI Dashboard

The interactive dashboard provides insights into:

- Injury Rate
- Injury by Position
- Injury by Match Load
- Injury by Training Level
- Injury by Sleep Category
- Injury by Nutrition
- Injury by Previous Injury History
- Correlation Analysis
- Key Performance Indicators (KPIs)

> Add your dashboard screenshot here.

```text
/dashboard/dashboard.png
```

---

# 🤖 Machine Learning

### Algorithm

- K-Nearest Neighbors (KNN)

### Workflow

- Label Encoding
- Feature Selection
- Standard Scaling
- Train/Test Split
- Hyperparameter Tuning
- Model Training
- Model Evaluation

---

# 📊 Model Performance

Evaluation Metrics:

- Accuracy
- Confusion Matrix
- Classification Report

> Add your evaluation screenshots here.

---

# 🌐 Deployment

The trained K-Nearest Neighbors (KNN) model was deployed using **Gradio**, allowing users to interact with the model through a simple web interface.

### 🔗 Live Demo

👉 **Try the application here:**  
[https://your-gradio-link.gradio.live](https://66343f5f9cdb502fc1.gradio.live)

### Features

- Select the player's position.
- Enter the player's fitness and performance metrics.
- Predict whether the player is likely to suffer an injury in the next season.

> **Note:** The prediction is intended for educational purposes and is based on the provided dataset.

---

# 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Gradio
- Joblib
- Power BI

---

## ⭐ If you found this project useful, don't forget to give it a Star.
