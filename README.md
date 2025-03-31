# credit-risk-classification

Supervised learning using a Logistic Regression mdoel and fit to training data in order to test the testing data to classify healthy loans (0) and high risk loans (1). 

Confusion Matrix:

<img width="135" alt="Screenshot 2025-03-31 at 1 33 33 PM" src="https://github.com/user-attachments/assets/07b703b6-5c3f-44c6-a125-792099f10361" />

Classification report:

<img width="398" alt="Screenshot 2025-03-30 at 10 56 56 PM" src="https://github.com/user-attachments/assets/87c2c8c4-0922-4aec-bd21-71295a4d90b3" />

- Accuracy: The logistic regression moodel has 99% accuracy (true pos+true neg)/total (56015+1739)/(56015+103+1739+295)=57754/58152
- Precision: The ratio of correctly predicted to all predicted for a class (true pos/(true pos+false pos))
    For healthy loans, the precision is approximately 100% (56015/(56015+103)=56015/56118)
    For risky loans, the precision is 85% (1739/(1739+295)=1739/2034)
- Recall: The ratio of correctly predicted to all the values that should have been in the class (true pos/(true pos+false neg))
    For healthy loans the recall is 99% (56015/(56015+295)=56015/56310)
    For risky loans the recall is 90% (1739/(1739+103)=1739/1842)

If the company provides mostly smaller loans with less risk when lending then the model may suffice with such a high recall and precision for selecting healthy loans. However, if the company provides higher loans with a higher risk for loss, the 85% precision and 90% recall for discerning which loans are risky may not be high enough to confidently move forward with and more data may need to be collected to predict a risky loan. 
