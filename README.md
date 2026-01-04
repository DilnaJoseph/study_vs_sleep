📊 Sleep vs Study: Are All-Nighters a Myth or a Miracle?

📌 Project Overview

This project analyzes how sleep hours, study hours, and stress levels affect a student’s exam score.
Using exploratory data analysis (EDA) and a regression model, we aim to answer a popular student dilemma:

```Do all-nighters actually help, or does sleep matter more than we think?```

🎯 Objectives

   - Predict student exam scores using:
     
      - Sleep Hours
      - Sleep difficulty
      - Sleep Quality
      - Concentration
      - fatigue
      - Classes missed
      - Caffeine consumption
      - Physical activity
      - Study Hours
      - Stress Level
        
  - Analyze relationships between sleep, study habits, stress, and performance
  - Evaluate model performance using standard regression metrics

📊 Dataset

Custom survey dataset (data.csv) containing responses from students about their:

  - Sleep patterns (duration, quality, difficulties)
  - Study habits and academic stress
  - Lifestyle factors (caffeine, exercise, screen time)
  - Academic performance (self-reported grades)

🔬 Methodology

1. Data Preprocessing

  - Encoding: Ordinal mapping for categorical variables (e.g., "Poor" → 1, "Excellent" → 5)
  - Cleaning: Removed timestamp, handled missing values
  - Feature Selection: Correlation-based selection (threshold: 0.05)

2. Exploratory Data Analysis (EDA)

EDA was performed to identify patterns and trends, including:
  - Correlation heatmaps
  - Distribution analysis (box plots, violin plots)
  - Cross-tabulation of sleep vs. performance
  - Statistical summaries by sleep/stress groups
   
3. Model Training

Trained and compared 7 regression models:

  - Linear Regression (baseline)
  - Ridge Regression (α = 0.1, 1.0, 10)
  - Random Forest (depths: 5, 10, 15)

4. Evaluation Metrics:

  - R² Score (test & cross-validation)
  - Mean Absolute Error (MAE)
  - Prediction accuracy (within ±0.5, ±1.0 grades)

    
Performance Summary
  - The model achieves a reasonable R², indicating good explanatory power.
  - MAE is low enough to confirm practical usability.
  - Results show that balanced sleep + study leads to the best outcomes.
