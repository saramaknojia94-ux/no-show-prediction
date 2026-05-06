# Patient No-Show Prediction

I started this project after noticing how much operational damage 
missed appointments cause in clinical settings — wasted provider 
time, scheduling gaps, downstream care delays. Wanted to see if 
appointment data alone could flag high-risk no-shows before they 
happen.

## The Question
Can we predict which patients are likely to miss their appointment 
— and which factors matter most?

## Data
110k+ medical appointments from Brazil via Kaggle.
Source: https://www.kaggle.com/datasets/joniarroba/noshowappointments

## Approach
- Exploratory data analysis to understand no-show patterns
- Feature engineering (wait time, day of week, patient history)
- Logistic Regression baseline
- XGBoost for improved performance
- SHAP for explainability — understanding WHY a patient is flagged

## Tools
Python, pandas, scikit-learn, XGBoost, SHAP, Matplotlib

## Status: Complete

## Key Results
- XGBoost ROC-AUC: 0.721
- No-show recall: 79% (catching 8 out of 10 no-shows)
- Top predictor: wait time (SHAP value 0.817)
- Logistic Regression baseline AUC: 0.655
