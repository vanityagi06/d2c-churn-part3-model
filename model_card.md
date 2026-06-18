# Model Card
## Model Name
Customer Churn Prediction Model

## Model Type
Binary Classification
Algorithms Evaluated:
* Logistic Regression (Baseline)
* Random Forest Classifier (Final Model)

## Intended Use
The model predicts the probability that a customer will churn within the next 60 days.
The output is intended to support:
* Retention campaign prioritization
* Customer success outreach
* Marketing budget allocation

## Data Sources
* customers.csv
* orders.csv
* support_tickets.csv
* web_events_snapshot.csv
* intervention_history.csv
* rfm_modeling_snapshot.csv

Snapshot Date:
2025-09-30

Target Window:
60 days after snapshot date.

## Features Used
Examples:
* recency_days
* frequency_180d
* monetary_180d
* return_rate_180d
* ticket_count_90d
* sessions_30d
* campaign_clicks_30d
* last_visit_days_ago

## Performance
Evaluation metrics are stored in metrics.json.

Metrics evaluated:
* Accuracy
* Precision
* Recall
* F1 Score
* ROC AUC
The Random Forest model outperformed the baseline Logistic Regression model and was selected as the final model.

## Limitations
1. Model performance depends on historical customer behavior.
2. Sudden customer preference changes may not be captured.
3. External market conditions are not included.
4. The model does not explain all reasons behind churn.

## Ethical Considerations
* Predictions should assist decision-making, not replace human judgment.
* Customers should not be penalized solely based on churn predictions.
* Marketing interventions should remain fair and non-discriminatory.

## Monitoring Requirements
The following should be monitored after deployment:
* Prediction distribution
* Data drift
* Feature drift
* Model performance degradation
* Retention campaign outcomes

Retraining should occur whenever significant performance degradation is observed.
