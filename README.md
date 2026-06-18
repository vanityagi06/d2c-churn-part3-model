# D2C Customer Churn Intelligence - Part 3
## Objective
Build a machine learning model capable of predicting customer churn within the next 60 days.
## Files Included
* churn_model.ipynb
* model.pkl
* metrics.json
* error_analysis.md
* model_card.md
* requirements.txt

## Methodology
### Data Source
rfm_modeling_snapshot.csv

### Models Trained
1. Logistic Regression (Baseline)
2. Random Forest Classifier (Final Model)

### Evaluation Metrics
* Accuracy
* Precision
* Recall
* F1 Score
* ROC AUC

### Feature Importance
Feature importance analysis was performed using the Random Forest model to identify the strongest drivers of churn.

## Outputs
* Trained machine learning model
* Evaluation metrics
* Feature importance analysis
* Error analysis
* Model card

## How to Run
Install dependencies:
pip install -r requirements.txt
Open and execute:
churn_model.ipynb
## Author
Vani Tyagi
