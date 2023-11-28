# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Lending entities extend financial resources or assets to borrowers with the expectation that the borrower will either return the asset or fulfill the loan repayment. The concept of credit risk emerges when a borrower falls short in returning the asset or repaying the loan, leading to potential financial losses for the lender. Lenders employ diverse metrics to gauge this risk. In the context of this Module, we will leverage Machine Learning methodologies to scrutinize a dataset encompassing historical lending transactions from a peer-to-peer lending services company. The ultimate aim is to construct a model proficient in discerning the creditworthiness of borrowers.

Employing a machine learning model, I aim to discern the health status of loans—categorized as either low-risk (healthy) or high-risk (non-healthy)—based on the loan status provided by the lending company.

The Logistic Regression Algorithm has been selected as the optimal tool for our machine learning model, given its widespread application in predicting the probability of a target variable in classification problems.

Upon utilizing the dataset furnished by the lending company, I constructed a Logistic Regression Model that yielded an impressive accuracy score of 95%. Notwithstanding this high accuracy, it is noteworthy that the model's recall value for non-healthy loans stands at 0.91, which is comparatively lower than the recall value of 0.99 for healthy loans. This discrepancy implies that the model exhibits a greater proficiency in predicting loan statuses as healthy rather than non-healthy. The underlying cause can be attributed to dataset imbalance, where one class label (in this instance, healthy loans) significantly outweighs the other (non-healthy loans).



## Results

* Machine Learning Model 1: Logistic Regression Model fitted with Imbalanced Data
  * According to the classification report, it predicts healthy loans (0) 100% of the time, while it predicted high-risk loans     (1) 85% of the time.
  * Since this model has imbalanced data, it has a higher probability of making mistakes

 ![imbalanced_data](https://github.com/dahmadi/CreditRisk/blob/8f45320577216c99f391669cf096d2834b5d27dd/Module%2012%20Images/Imbalanced%20Data%20Report.png)
    
* Machine Learning Model 2: Logistic Regression Model fitted with Balanced (oversampled) Data 
  * The Logistic Regression model fitted with the OverSampled DataSet predicted healthy loans (0) 100% of the time and             predicted non-healthy (1) loans 84% of the time.
  * the model made 1% of mistakes when predicting healthy loans and made 1% of mistakes when predicted non-healthy loans.
  * The model generated an accuracy score of 99% due to the dataset being balanced.

## Summary

The Logistic Regression model, trained on Oversampled data, exhibited superior performance compared to the model trained on Imbalanced data. This improvement is attributed to the balanced nature of the data, resulting in a higher accuracy score and an elevated recall. These outcomes suggest that the model is poised to minimize errors significantly when classifying non-healthy loans.

For the lending company, reducing False Positives is crucial, given the heightened risk of financial loss when misclassifying non-healthy loans as healthy. The ensuing data is presented in the confusion matrices, offering insights into the model's accurate and inaccurate predictions of healthy and non-healthy loans.

I would recommend using Model 2 Logistic Regression Model fitted with Balanced data.
