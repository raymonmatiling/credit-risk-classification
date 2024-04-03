# credit-risk-classification

## Overview of the Analysis

* The purpose of the analysis was to develop and evaluate machine learning models for credit risk assessment using historical lending data. The dataset comprised financial information from a peer-to-peer lending services company, including borrower characteristics and loan status. The main task was to predict loan default risk based on this information. The target variable, "loan_status," had two classes: 0 for healthy loans and 1 for high-risk loans. The analysis involved several stages of the machine learning process, including data preparation, model development, and evaluation. Initially, the dataset was prepared by extracting features and labels. Then, logistic regression, a popular classification algorithm, was employed to build the predictive model. Other stages included splitting the data into training and testing sets, training the model on the training set, and evaluating its performance using metrics such as accuracy, precision, and recall. The logistic regression algorithm was chosen due to its simplicity and interpretability, making it suitable for initial analysis and baseline performance evaluation.

## Results

* Machine Learning Model:
  * Accuracy - The logistic regression model demonstrates an overall accuracy rate of approximately 96.32%. It correctly predicts 18,663 instances of healthy loans and 563 instances of high-risk loans out of the total dataset. This indicates that the model correctly predicts the majority of both healthy loans (label 0) and high-risk loans (label 1) from the total dataset.

  * Precision - Precision measures the model's ability to correctly identify positive cases among all instances predicted as positive. For healthy loans, the precision is at its highest value of 1, indicating that nearly all predicted healthy loans are indeed healthy. However, for high-risk loans, the precision slightly drops to 0.85, implying that around 15% of the predicted high-risk loans are misclassified.

  * Recall - Recall evaluates the model's capability to capture all actual positive cases. The recall for healthy loans is exceptionally high at 0.99, suggesting that the model effectively identifies almost all actual healthy loans. Conversely, for high-risk loans, the recall is 0.91, indicating that approximately 9% of actual high-risk loans are not identified by the model.
  
## Summary

Based on the analysis of the machine learning models, the logistic regression model shows a strong performance in predicting healthy loans (label 0) with high precision and recall scores. However, its performance in identifying high-risk loans (label 1) is less satisfactory, as indicated by lower precision and recall scores for this class. This discrepancy suggests that the logistic regression model struggles to accurately identify high-risk loans, which are crucial for minimizing potential financial losses.

In terms of which model performs best, it depends on the specific problem being addressed. If the primary objective is to minimize the misclassification of high-risk loans (label 1), then a model with high precision and recall for label 1 would be preferable. Conversely, if overall accuracy and reliability in predicting loan status regardless of class are the main concerns, then a model with balanced precision and recall scores for both classes would be desirable.

Considering the limitations of the logistic regression model in accurately predicting high-risk loans, further model refinement or exploration of alternative algorithms may be necessary to improve performance, particularly for label 1 predictions. Without significant improvement in accurately identifying high-risk loans, it may not be advisable to rely solely on the logistic regression model for credit risk assessment. Therefore, caution should be exercised before deploying the model for operational use in its current state, and consideration should be given to exploring alternative models or implementing additional feature engineering to enhance performance.




