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

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
