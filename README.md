# credit-risk-classification
- - -

## **Background:**
This project was created as part of a data anlaytics bootcamp. The goal is to use Python and supervised learning to build a model that can identify the creditworthiness of borrowers using a dataset of historical lending activity from a peer-to-peer lending services company.

Relevant Files:
- [Credit Risk Classification Jupyter Notebook](Credit_Risk/credit_risk_classification.ipynb)
    -The data analysis is completed in this notebook.
- Resources
  - [lending_data.csv](Resources/lending_data.csv)
  -This data was provided as part of the exercise. 


## **Part 1: Splitting the Data into Training and Testing Sets**
I loaded the csv file into a Pandas dataframe, and from there split the data into training and testing sets. 

## **Part 2: Create a Logistic Regression Model with the Original Data**
I then used logistic regression to predict each loan applicant's classification as high-risk or low-risk. I created a confusion matrix to validate the model. 

#### Confusion Matrix:
          predicted 0  predicted 1
    actual 0        18679           80
    actual 1           67          558


#### Accuracy Score:
    0.9442676901753825


#### Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      0.89      0.88       625

    accuracy                           0.99     19384
    macro avg       0.94      0.94      0.94     19384
    weighted avg       0.99      0.99      0.99     19384



## **Part 3: Create a Logistic Regression Model with Oversampled Data**
Because high-risk applicants are underrepresented in the original data, I built a 2nd logistic regression model using oversampled data. This increased the number of high-risk applicants relative to low-risk. The result was a model that can better predict who should be classified as high-risk. 

####Confusion Matrix:
          predicted 0  predicted 1
    actual 0        18668           91
    actual 1            2          623


####Accuracy Score:
    0.9959744975744975


Classification Report:
              precision    recall  f1-score   support

           0       1.00      1.00      1.00     18759
           1       0.87      1.00      0.93       625

    accuracy                           1.00     19384
    macro avg       0.94      1.00      0.96     19384
    weighted avg       1.00      1.00      1.00     19384



- - -

## How to Run the App

1. Clone the repo to your computer.
   - [How to Clone Github Repo](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository)

2. Open the Credit-Risk-Classification folder in VS Code on your personal computer.

3. Navigate to the [Credit Risk Classification Jupyter Notebook](Credit_Risk/credit_risk_classification.ipynb) file in the folder.

4. Connect to your kernal. 

5. Run all cells. 