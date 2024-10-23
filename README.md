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
![](images/DataDictionary.png)

2. 
3. Random Forest Model Creation
4. Sample decision tree from random forest

## Results and Model Evaluation

### Results and Model Evaluation:

From a security perspective, we want to avoid predicting a phishing URL as safe (False Negative), so **Recall** is the most important measure for this model. This ensures that the model identifies all phishing URLs accurately, minimizing the chances of missing any malicious threats that could compromise user security.

Since the model produces very similar recall scores on both the training and testing data, it demonstrates strong performance, maximizing its ability to detect phishing URLs without overfitting to the training data or sacrificing its generalizability to new, unseen URLs.

- **Recall**: Recall on the testing data is 99%, meaning that the model successfully detects all phishing URLs. This ensures that no phishing attempts are missed.

- **Precision**: Precision on the testing data is 99%, indicating that there are relatively few False Positives (legitimate URLs flagged as phishing). While precision is important, our priority is catching all phishing URLs to avoid security breaches.

- **Accuracy**: Accuracy on the testing data is 99%, meaning that the model correctly classifies 4 out of 5 URLs as either phishing or legitimate.

- **F1 Score**: The F1 score on the testing data is 99%, reflecting a good balance between precision and recall, with the model managing both False Positives and False Negatives effectively.

### Future Utilization and Implementation:

Now that the model has been developed and evaluated, the next step is to **integrate it into security platforms** to actively detect and block phishing URLs in real-time. As a basic implementation, the model can be used in a **web application** where security teams or end-users can input URLs to check for phishing threats. However, there are additional advanced steps to take:

1. **Web Application Integration**: Implement the model in a simple web app where users can submit URLs and get instant feedback on whether a URL is potentially phishing. This basic step will help in day-to-day phishing detection tasks.

2. **Incorporation with a Search Engine**: To take the model further, it can be incorporated into a **search engine** to provide real-time phishing detection for URLs indexed by the engine. For example, the model could flag or remove phishing URLs before they even show up in search results, significantly reducing the chances of users encountering harmful sites.

3. **Browser Extensions**: Another way to utilize the model would be to create a **browser extension** that warns users when they are about to visit a potentially malicious website. This extension could scan URLs as they are visited and provide immediate feedback based on the model’s predictions.

4. **Email Filters**: Phishing URLs are often delivered via email, so integrating this model into an **email security filter** would allow the model to analyze URLs embedded in emails and quarantine or block phishing attempts before they reach the user.

5. **Security Information and Event Management (SIEM)** Platforms: For enterprise-level security, the model can be incorporated into **SIEM systems** to monitor web traffic and flag phishing URLs in real-time across a network. This would allow for automated detection of phishing URLs before they reach the end user.

### Business Impact:

Once deployed, this model will greatly enhance security measures by detecting phishing URLs in real-time, preventing users from accessing malicious sites. Whether integrated into a web application, search engine, or browser extension, the model will help reduce phishing attacks, protect sensitive information, and improve overall cybersecurity.

### Next Steps:

1. **Implement the model in a web app** to allow for initial phishing detection capabilities.
2. **Explore integrations with search engines, browser extensions, and SIEM platforms** to broaden the impact and functionality of the model.
3. Continuously **monitor and retrain the model** as new phishing URLs are discovered, ensuring it stays up-to-date and effective at detecting emerging threats.
