# Credit-Card-Fraud-Detection
Identify fraudulent credit card transactions.

# Description 
Credit card companies should be to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase.However, it is an extremely challenging task as there might be only 1000 fraud cases in over a million transactions, representing a meager 0.1% of the dataset, leading to highly imbalanced datasets. The ML algorithms are very likely to produce faulty classifiers when they are trained with imbalanced datasets as they tend to show a bias for the majority class, treating the minority class as a noise in the dataset. Also, due to the class imbalance "accuracy" is not a meaningful metric for unbalanced classification. The algorithm would be able to predict almost all cases belonging to the majority class which will yield a high accuracy score. However, the minority class would be totally ignored by the algorithm. The Accuracy Score would give a false sense of security to the credit card companies which can cost individuals and businesses lots of money. 

# Dataset
The dataset used in this project have 492 fraudulent transactions out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for only 0.172% of all transactions. The dataset is available for download at https://www.kaggle.com/mlg-ulb/creditcardfraud

# Algorithms
I have used three classification algorithms namely Logistic Regression CV, Random Forest Classifier and XGBoost Classifier. I have trained the classifier using the original dataset and a dataset obtained after performing Synthetic Minority Over-Sampling Technique (SMOTE) on the original dataset. I have split the data into training and test set at a ratio of 70:30. 

# Metrics Used to Evaluate Classifier Performance
I have used F1 Score, Recall, Precision, Confusion Matrix, Average precision-recall score and Average ROC_AUC score as metrics to evaluate the classifiers as they give a better indication of the model compared to accuracy.

# Results
The Logistic Regression gives the best Recall score on the original dataset among the three algorithms. However, it lags the other two classifiers on all other metrics. XGBoost gives the best F1 score among the classifiers.
Using the classifiers on the SMOTE dataset improves the Recall of the models at the cost of Precision and F1 Score.
