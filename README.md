# Electricity_Fraud_Detection
This code Detect customers who are likely to be involved in Electricity Fraud.The output derive the probability of a Client involving in Fraud.High Probability mens highly likely to be involved in Fraud
README.md
This repository contains code for electricity fraud detection. The code is written in Python and uses various libraries for data manipulation, visualization, and machine learning.

Dependencies
The following libraries are required to run the code:

pandas (imported as pd)
numpy (imported as np)
seaborn (imported as sns)
matplotlib.pyplot (imported as plt)
warnings
Data
The code assumes that the following datasets are available in CSV format:

client_train.csv: Contains information about clients in the training set.
invoice_train.csv: Contains information about invoices in the training set.
client_test.csv: Contains information about clients in the test set.
invoice_test.csv: Contains information about invoices in the test set.
The datasets are loaded into DataFrames using the pandas library.

Usage
The code provided performs the following steps:

Read the client_train.csv and invoice_train.csv datasets into DataFrames named client_train and invoice_train, respectively.
Read the client_test.csv and invoice_test.csv datasets into DataFrames named client_test and invoice_test, respectively.
Merge the invoice_train and client_train DataFrames on the client_id column, creating a new DataFrame named df.
Merge the invoice_test and client_test DataFrames on the client_id column, creating a new DataFrame named df1.
Perform exploratory data analysis on the df DataFrame, including checking its shape, size, information, and descriptive statistics.
Calculate the correlation matrix of the df DataFrame and visualize it using a heatmap.
Import additional libraries required for fraud detection, such as mean_squared_error, accuracy_score, roc_auc_score, LabelEncoder, OneHotEncoder, IsolationForest, lightgbm, xgboost.
Prepare the input features (X) and target variable (y) for the machine learning model by dropping unnecessary columns from the df DataFrame.
Convert categorical columns in the df DataFrame to the category data type.
Train a machine learning model on the prepared data.
Conclusion
This code provides a starting point for electricity fraud detection using machine learning techniques. It demonstrates how to load and preprocess the data, perform exploratory data analysis, and train a fraud detection model. Feel free to modify and extend the code according to your specific requirements.

Note: The code assumes that the required datasets are available in the specified format. Please make sure to adjust the file paths or data loading code accordingly if necessary.






