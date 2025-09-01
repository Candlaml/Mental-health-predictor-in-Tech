# 🧠 Mental Health in Tech: Predictive Modeling & Workplace Insights

## Overview

This project explores mental health challenges in the tech industry using data-driven analysis and machine learning. By examining workplace culture, personal history, and demographic factors, we aim to build predictive models that help HR teams identify at-risk employees and foster supportive environments.

## Objectives

- Analyze patterns in mental health responses across age, gender, company size, and workplace support
- Apply sampling strategies to address class imbalance in mental health status
- Train and evaluate multiple classification models to predict mental health outcomes
- Prioritize fairness, recall, and interpretability in model selection
- Provide actionable insights for mental health interventions in tech workplaces

## Dataset

- **Source**: 2017 Workplace Mental Health Survey  
- **Size**: ~750 responses, 123 features  
- **Target Variable**: `mental_health` (4 classes: Yes, Possibly, No, Don’t Know)

## Exploratory Data Analysis (EDA)

- Age 30–35 group shows highest mental health concern
- Mid-sized (100–500) and large (1000+) companies report most “Yes” responses
- Perceived coworker reactions and observed support strongly correlate with mental health status
- Family history and prior diagnosis are key predictors
- Diagnosis drives acknowledgment, but many remain undiagnosed

## Modeling Approach

- Models used: Logistic Regression, Random Forest, XGBoost, KNN, VotingClassifier, Tuned Random Forest
- Sampling strategies: None, Normalization, Oversampling, Undersampling, SMOTE
- Evaluation metrics: F1 Score, Recall, PR-AUC (prioritized), Accuracy, ROC-AUC

## Key Results

- **Best Model**: Tuned Random Forest with Oversampling  
  - F1 Score: 0.8102  
  - Recall: 0.8092  
  - PR-AUC: 0.795  
- VotingClassifier also performed strongly, especially in PR-AUC

## Why It Matters

Mental health is a growing concern in tech, where high pressure and low support can lead to burnout and silence. This project helps organizations move beyond generic wellness programs toward data-informed, empathetic interventions.

## How to Use

1. Clone the repository  
2. Run `eda.ipynb` for exploratory analysis  
3. Run `modeling.ipynb` to train and evaluate models  
4. Review `results_summary.xlsx` for performance comparison  
5. Use insights to inform HR strategies and mental health initiatives

## Contributors

- **Lead Analyst**: Candela Medina, Helin 


## License

This project is open-source and intended for educational and ethical use. Please cite responsibly and respect the sensitivity of mental health data.

## Future Research

Adding data from more years. Due to time restrictions only data from the 2017 surveys were used.

