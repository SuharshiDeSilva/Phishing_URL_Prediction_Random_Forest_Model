# Phishing_URL_Prediction_Random_Forest_Model

Phishing attacks represent a significant aspect of cybersecurity attacks involves in deceiving users into revealing sensitive information by posing as legitimate entities through fraudulent platforms. They have grown in sophistication and frequency, targeting individuals and organisations and resulting in significant financial and data losses. This research project aims to contribute to the fight against such attacks by developing a robust ML model for detecting phishing Websites.

## Project Objective

- To find a suitable balanced dataset to create reliable ML model.
- To implement a comprehensive data preparation process with feature selection, dimensionality reduction, and data cleaning to enhance the model performance.
- To identify and build a predictive model using ML techniques for detecting phishing URLs.

## Business Case

To create a model that accurately predicts phishing URL.

## Goal
To accurately predict phishing URL without falsely predicting phishing URLs which could affect the users. 

## Deliverables

### In Repository:
1. Data& Data Dictionary
2. Random Forest Model Creation
3. Sample decision tree from random forest

## Results and Model Evaluation

From a business perspective, we want to avoid predicting a positve loan approval when it was actually denied (False Positives), so Precision will be our best measures for the model. This will ensure that we are accurately predicting loan approvals and that predicted approvals are actual approvals (precision).

Since this model produces very similar precision scores on both the training and testing data, it appears to be the best fit to maximize predictive power on the training dataset without overfitting and sacrificing predictability on the testing data.

Precision: Precision on the testing data is ~78%, which means that we don't have a large amount of False Positives. This is great, because as a business, we want to avoid predicting loans approvals that will have to be denied later.

Accuracy: Accuracy on the testing data is ~80% which means that the model correctly predicts 4/5 of the loans.

Recall: Recall on the testing data is 100% which means that the model accurately predicts all True Positives. This means that we will not miss out on any potential loan approvals (and revenue).

F1 Score: The F1 score on the testing data is ~88%, which is great since it takes into account both False Positives and False Negatives.

## Business Impact

## Next Steps
