# Loan-Prediction-Gradient-Boosting-Machine-Learning
Automate the Loan eligibility process using Gradient Boosting Ensembler

Dataset obtained from Analytics Vidhya

We are given train and test dataset. The aim is to automate the loan eligibility process based on the details provided by the customers.

The project is divided into following parts:

  1. Data Cleaning (Fill the null and empty values appropriately)
  2. Data Visualization
  3. Apply one of the ensembler : Gradient Boosting or Random Forest
  4. Train the model using the ensembler Machine Learning Algorithm
  5. Predict the values for the test data
  
We chose Gradient Boosting Algorithm to impute the missing values. In GBM, the predictors are selected incrementally resulting in low bias and variance. Subsequent predictors learn from the mistakes of the previous predictors.

We plotted univariate and multivariate plots to get the significance of each feature and the relation between each attribute. For the multivariate plot, we find heatmap more useful to know the relationship among the attributes.

The dataset given to us was uncleaned and filled with wrong input. First, in order to anaylze the data, we cleaned and imputed the empty entries. 

Relationship between "Loan_Status" and all the other attributes using Count Plot using Seaborn library.

Split the data into training and test data using model selection from Sklearn library.

Performed Gradient Boosting Classifier on th train data set with various n_estimators and learning rate and choosing the one with the best accuracy.

Beware from overfitting the model. We might get high accuracy using the training data but that might not be the case with test data set.

Choosing of number of estimators and learning rate is crucial for the model to be successful.

With appropriate parameters, we were able to predict the Loan_Status of the customers on the test dataset.
