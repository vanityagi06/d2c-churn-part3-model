# Error Analysis
## Objective
The purpose of error analysis is to understand where the churn prediction model makes incorrect predictions and identify opportunities for improvement.

## False Positives
False Positives are customers predicted to churn but who were actually retained.

### Possible Reasons
* Temporary inactivity before making a purchase.
* Seasonal purchasing behavior.
* High engagement but low recent transaction frequency.
* Customers responding positively to previous retention campaigns.

### Business Impact
False positives may result in unnecessary retention spending, but generally have lower business risk than false negatives.

## False Negatives
False Negatives are customers predicted to remain active but who actually churned.

### Possible Reasons
* Sudden changes in customer preferences.
* Negative experiences not captured in available features.
* External market influences.
* Competitor promotions and switching behavior.

### Business Impact
False negatives are more costly because churned customers receive no intervention.

## Example Customer Reviews

### Customer CUST01071
Prediction Review:
Customer displayed moderate engagement but uncertain purchasing behavior.

### Customer CUST00102
Prediction Review:
Limited transaction history resulted in ambiguous risk signals.

### Customer CUST00252
Prediction Review:
Strong historical value but increasing inactivity.

### Customer CUST00325
Prediction Review:
Moderate spending and average engagement patterns.

### Customer CUST01705
Prediction Review:
High browsing activity but inconsistent purchasing.

### Customer CUST00223
Prediction Review:
Long recency period increased churn risk.

### Customer CUST01285
Prediction Review:
Historically loyal customer with declining activity.

### Customer CUST00850
Prediction Review:
Insufficient purchase history for confident classification.

### Customer CUST00756
Prediction Review:
Extended inactivity suggested elevated churn risk.

### Customer CUST01926
Prediction Review:
Low spending and low engagement increased uncertainty.

## Recommendations
1. Incorporate additional behavioral features.
2. Track campaign response effectiveness.
3. Include customer lifetime value signals.
4. Periodically retrain the model to address changing customer behavior.
