# All-Lending-Club-Loan-Data
 Jupyter notebook
 I achieved precision of 88%, but it should be more, in lecture https://www.udemy.com/course/python-for-data-science-and-machine-learning-bootcamp/learn/lecture/17739848#questions, the obtained precision was 97%, because of preprocessing and feature engineering.
 
 Points to be noted-
 1. use one hot encoding instead of label encoder
 2. using columns like issue_d was a data leakage, so domain knowledge is important for choosing columns while training
 3. many columns have same meaning or provides same information
 4. normalisation should be done at the very last , just before training model, and it should not be done one by one for every column, but for whole dataframe
 5. due to inbalance in dataset itself, the model has only around 90% accuracy
 6. for ann if data is very large, use only 25-50 epochs, and batch size should be more to avoid overfitting on large data
 7. for ann if ram of device is less, then sample 10% of data and then train
