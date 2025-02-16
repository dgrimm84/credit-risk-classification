# credit-risk-classification

<ins>Analysis Overview:</ins>

The purpose of this analysis is to summarize the findings made by the Logistic Regression Model.  The model was tested and trained to look at the loan_status column of the dataset and predict where each row of data will fall in each category.  This summary of the dataset will allow companies like banks, credit unions, or loan companies to make a much more efficient, educated estimate on the number of loans in this list that are healthy and which are high-risk to protect the company's assets.  

<ins>Analysis Results:</ins>

-	The confusion matrix shows a very high True Negative of 55,987 (correctly predicting healthy loans, a zero) and a very high True Positive of 1,754 (correctly predicting loans with a high likelihood of defaulting, a one).  It also shows comparatively very low False Positives (predicting unhealthy loans as healthy loans incorrectly) and False Negatives (predicting healthy loans as unhealthy loans incorrectly). This means that the model was able to predict a much higher number of true 0s and true 1s with the majority being 0s.

-	The classification report reinforces the much higher count and much higher percentage of correctly-predicted healthy loans represented by a 0 in the dataset.The precision rate of predicting a healthy loan was 100% while the precision rate of predicting a high-risk loan was only 86%.  This is biased towards the prediction of healthy loans.

    - Also, the classification report shows a recall score of 0.99 for healthy loans and 0.93 for high-risk loans.  This means that 99% of actual healthy loans were correctly identified while 93% of actual high-risk loans were correctly identified.
    - Finally, the  f1-score is the ratio relationship between the recall and precision of the  model.  Healthy Loans (0) has a perfect score of 1.0 and High Risk loans has an OK score of 0.90; which definitely has room for improvement.

<ins>Analysis Summary:</ins>

Using all the report results generated from the Logistics Regression model, we are able to determine that the model predicts healthy loans better and more commonly than loans with a high likelihood of default.  I would recommend this model to a loan company beacuse of the high accuracy of predicting healthy loan statuses.  However, beacuse of the relatively low precision, count, recall, and prediction of high-risk loans, there does seem to be some missing data from the dataset to give an accurate representation of loans that have a high chance of going into default.  

## The files in this directory and their function

credit_risk_classification.ipynb is the main code file for this project.  The functions that this file completes are:
  - the file Resources/lendingdata.csv is imported into python and a dataframe is created
  - labels for the regression model X and y are created from the loan_status column showing a "0" for a healthy loan and "1" for a high-risk loan
  - this dataframe is split into testing and training data using these two variables
  - this training data is fit into a Logistic Regression Model to perform this analysis
  - after this model is run, the testing data predictions from X_test are saved to be printed in analysis models later
  - a confusion matrix is created to show the True Positive, True Negative, False Positive, and False Negative results

    ![image](https://github.com/user-attachments/assets/d8aba413-4524-48cb-b180-9b5053413c56)

- Then, a classification report is created to show the precision, recall, f1-score, and support results from this prediction/regression model

  ![image](https://github.com/user-attachments/assets/de5b5a36-f488-4a7f-899b-c488a4a375f0)


