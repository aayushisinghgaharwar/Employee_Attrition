# Employee_Attrition


Purpose: 
Aim to perform analysis to figure out the likelihood of an active employee leaving the company and the key indicators surrounding it.

Approach:
Made predictions on the time period when employees will end the job, understanding the main drivers of employee churn.
Tried to delve deep in the dataset to identify patterns and trends in the dataset.
Used feature engineering to create new features in order to enhance modeling.
Created a variable “EXPERIENCE_AT_COMPANY” based on the number of years of experience that a person has in the past five years at the company.
Used PCA (Principal Component Analysis) is performed on dataset after removing two columns: EMP_ID and TERMINATION_YEAR. It is done using 116 columns.

Results:
From the PCA, we infer that 106 out of 116 are ideal for explaining 100% variance. But the accuracies are not high. So, PCA not useful.
In Random Forest, there was high accuracy. Hyperparameters are “max_depth” of 20 & “n_estimators” as 100.
In Logistic Regression, “ANNUAL_RATE” and “HRLY_RATE” decreased accuracy by 2 percent.
In Decision Trees, “ANNUAL_RATE” was removed as it correlated with “HRLY_RATE”.
The KNN and the Naive Bayes models have performed equally. Removing a lot of features didn’t reduce the accuracy below 60%.

Conclusion:
After applying a lot of models for analysis, the boosting algorithms predict the maximum accuracy and the analysis state that factors which are the
most influential ones causing attrition are:
1. Job_Groups
2. Performance
Ratings
3. Job Code
4. Experience
5. Annual Rate
  
