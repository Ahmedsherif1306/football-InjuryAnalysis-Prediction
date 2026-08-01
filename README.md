# Football Injury Analytics & Prediction

An end-to-end Data Analytics and Machine Learning project that analyzes football player injury risk and predicts whether a player is likely to suffer an injury in the next season.

---

# Table of Contents

- [Project Mission](#project-mission)
- [About the Project](#about-the-project)
- [Objectives](#objectives)
- [Project Workflow](#project-workflow)
- [Dataset](#dataset)
- [Data Cleaning](#data-cleaning)
- [Feature Engineering](#feature-engineering)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Power BI Dashboard](#power-bi-dashboard)
- [Machine Learning](#machine-learning)
- [Model Performance](#model-performance)
- [Deployment](#deployment)
- [Technologies Used](#technologies-used)
- [Team Members](#team-members)
---

# Project Mission

Football injuries can negatively affect both player performance and team success. Identifying players who are at higher risk of injury helps coaches, medical staff, and performance analysts make informed decisions regarding training load, recovery, and injury prevention.

The mission of this project is to combine data analytics and machine learning to identify the key factors associated with football injuries, visualize injury patterns through an interactive dashboard, and build a predictive model that estimates injury risk for the next season.

This project demonstrates a complete end-to-end analytics workflow, from raw data preprocessing to dashboard development, machine learning, and deployment.

---

# About the Project

This project is an end-to-end Football Injury Analytics solution that combines data analysis, visualization, and machine learning.

The project includes:

- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Interactive Power BI Dashboard
- K-Nearest Neighbors (KNN) Classification
- Model Evaluation
- Gradio Deployment

The objective is not only to predict injuries but also to understand the factors that contribute to injury risk through data-driven analysis.

---

# Objectives

- Analyze the main factors affecting football injuries.
- Discover relationships between player fitness and injury risk.
- Build an interactive Power BI dashboard.
- Train a Machine Learning model to predict future injuries.
- Deploy the trained model using Gradio.

---

# Project Workflow

```text
Raw Dataset
      │
      ▼
Data Cleaning
      │
      ▼
Feature Engineering
      │
      ▼
Exploratory Data Analysis
      │
      ▼
Power BI Dashboard
      │
      ▼
Machine Learning (KNN)
      │
      ▼
Model Evaluation
      │
      ▼
Gradio Deployment
```

---

# Dataset

The dataset contains information for **800 football players**.

[**Football_injury data**](https://github.com/Ahmedsherif1306/football-injuryAnalysis-prediction/blob/main/Data/Raw_Data.csv)

## Features

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

## Target

**Injury Next Season**

- 0 → No Injury
- 1 → Injury

---

# Data Cleaning

[**Cleaned data**](https://github.com/Ahmedsherif1306/football-injuryAnalysis-prediction/blob/main/Data/Cleaned_data.csv)

The following preprocessing steps were performed:

- No missing values.
- No duplicate records.
- Verified BMI calculation.
- Converted **Position** into categorical values.
- Created new categorical features:
  - Training Level
  - Sleep Category
  - Nutrition Category
  - Match Load
  - Injury History
- Outliers were retained because they represent realistic player performance rather than data entry errors.

---

# Feature Engineering

Several new features were created to improve analysis and dashboard visualization:

- Training Level
- Sleep Category
- Nutrition Category
- Match Load
- Injury History

These engineered features simplify interpretation and make trends easier to visualize.

---

# Exploratory Data Analysis (EDA)

The exploratory analysis focused on understanding injury patterns and identifying the factors associated with injury risk.

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

# Power BI Dashboard

The project includes an interactive Power BI dashboard divided into four analytical pages, each focusing on a different aspect of football player performance and injury risk.

> **[Access the Live Power BI Dashboards Here](https://app.powerbi.com/view?r=eyJrIjoiNmRkOTRjNzUtNjgyMy00MzJkLTkwMTQtYTkzNzhmODNlNDdjIiwidCI6ImIzMDExMzJiLWMwNjYtNDk4MC1iMjU3LTdmZmRiOTdkNmY0NCJ9)**
> 

##  Overview Dashboard

This page provides a high-level summary of the dataset, including player distribution, injury statistics, and key performance indicators.



![OverView Dashboard](https://raw.githubusercontent.com/Ahmedsherif1306/football-injuryAnalysis-prediction/refs/heads/main/Dashboard/OverView_Page.png)

---

##  Performance Dashboard

This page analyzes players' physical performance through agility, sprint speed, balance, knee strength, reaction time, and flexibility across different player groups.

![Performance Dashboard](https://raw.githubusercontent.com/Ahmedsherif1306/football-injuryAnalysis-prediction/refs/heads/main/Dashboard/Performance_Page.png)

---

##  Training Dashboard

This page focuses on training habits and lifestyle factors such as training level, sleep, nutrition, stress level, and warm-up adherence.

![Training Dashboard](https://raw.githubusercontent.com/Ahmedsherif1306/football-injuryAnalysis-prediction/refs/heads/main/Dashboard/Training_page.png)

---

##  Injury Dashboard

This page investigates injury patterns by analyzing previous injury history, player position, nutrition, training level, and predicted injury risk.

![Injury Dashboard](https://raw.githubusercontent.com/Ahmedsherif1306/football-injuryAnalysis-prediction/refs/heads/main/Dashboard/Injury_page.png)
---
#  Key Insights

Based on the dashboard analysis:

- Players with **Frequent Previous Injuries** have the highest injury rate (**81%**), compared to **49%** for players with few injuries and **26%** for players with no previous injuries.
- Injury cases are distributed across all playing positions with only small differences, indicating that **position alone is not a strong predictor** of injury risk.
- Players with a **Moderate Training Level** represent the largest share of predicted injury cases, making this group the primary target for monitoring.
- The **Poor** nutrition category contains the highest number of predicted injury cases, while players with **Excellent** nutrition account for the fewest cases.
- Most players fall into the **Few Injuries** category, but those in the **Frequent Injuries** category exhibit a substantially higher injury rate.
- Physical performance metrics (agility, knee strength, balance, sprint speed, and reaction time) show measurable variation across training, nutrition, and recovery categories, highlighting their importance in evaluating player readiness.

---

#  Recommendations

Based on the dashboard findings:

- Prioritize medical monitoring for players with a history of frequent injuries.
- Develop individualized rehabilitation and injury-prevention programs for high-risk players.
- Improve nutrition plans to encourage players to reach higher nutrition quality levels.
- Combine physical performance assessments with injury history when evaluating player readiness.
- Use the injury prediction model as an early warning system to support coaching and medical staff in reducing injury risk.
- Monitor players experiencing **high stress levels**, since the dashboard indicates that increased stress is associated with a greater likelihood of injury. Mental recovery sessions and workload management should be incorporated into training plans.
- Encourage players to maintain **healthy sleep habits**, as poor sleep quality is linked to higher injury risk and reduced physical readiness. Coaches should promote consistent sleep schedules and adequate recovery time.

---

# Machine Learning

[**Predict_Injury Notebook**](https://github.com/Ahmedsherif1306/football-injuryAnalysis-prediction/blob/main/Notebook/Predict_injury.ipynb)

## Algorithm

- K-Nearest Neighbors (KNN)

## Workflow

- Label Encoding
- Feature Selection
- Standard Scaling
- Train/Test Split
- Hyperparameter Tuning
- Model Training
- Model Evaluation

---

# Model Performance

Evaluation metrics used:

- Accuracy
- Confusion Matrix
- Classification Report

---

# Deployment

[**Deployment Notebook**](https://github.com/Ahmedsherif1306/football-injuryAnalysis-prediction/blob/main/Deployment/app.ipynb)

The trained K-Nearest Neighbors (KNN) model was deployed using **Gradio**, allowing users to interact with the model through a simple web interface.

## Live Demo

**Try the application here:**

[https://66343f5f9cdb502fc1.gradio.live](https://522fa304ac6e98ecd1.gradio.live)

## Application Features

- Select the player's position.
- Enter the player's fitness and performance metrics.
- Predict whether the player is likely to suffer an injury in the next season.

**Note:** The prediction is intended for educational purposes and is based on the provided dataset.

---

# Technologies Used

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

If you found this project useful, consider giving it a ⭐ on GitHub.

---
## Team Members
<table align="center">
<tr>

<td align="center" width="33%">

<img src="https://github.com/Ahmedsherif1306.png" width="110"><br><br>

<b>Ahmed Sherif</b><br>

<i>Data Preprocessing & Machine Learning</i><br>

<a href="https://github.com/Ahmedsherif1306">GitHub</a>

</td>

<td align="center" width="33%">

<img src="https://github.com/eslam-zayed-eg.png" width="110"><br><br>

<b>Eslam Zayed</b><br>

<i>Deployment</i><br>

<a href="https://github.com/eslam-zayed-eg">GitHub</a>

</td>

<td align="center" width="33%">

<img src="https://github.com/ZeyadElshaboury.png" width="110"><br><br>

<b>Zeyad Elshaboury</b><br>

<i>Data Visualization</i><br>

<a href="https://github.com/ZeyadElshaboury">GitHub</a>

</td>

</tr>
</table>
