Credit Card Fraud Detection¶
Anonymized credit card transactions labeled as fraudulent or genuine

Feature Scaling
Concise Summary
Uique Labels
Descriptive Statistics
Finding null values
Distribution of Amount
Removal of Outliers
Categorical vs Continuous Features
Correlation Among Explanatory Variables
Feature Engineering
Feature engineering on Time
Scaling
Scale amount by Log
Scale amount by Standardization
Scale amount by Normalization
Saving preprossed data
Split data
Baseline for models
Class Imbalance
Under Sampling and Over Sampling
Synthetic Minority OverSampling Technique (SMOTE)
Adaptive Synthetic Sampling Method for Imbalanced Data (ADASYN)
Model Building
Logistic Regression
Logistic Regression with imbalanced data
Model Evolution
Model Evolution Matrix
Receiver Operating Characteristics (ROC)
Logistic Regression with Random Undersampling technique
Logistic Regression with Random Oversampling technique
Logistic Regression with SMOTE technique
Logistic Regression with ADASYN technique
Spatial nature of class imbalance
Distribution of balaced dataset
Distribution of balaced dataset
Building different models with different balanced datasets
Undersampled Data
Oversampled Data
SMOTE Data
ADASYN Data
Grid Search
Grid Search with Logistic Regression
Grid Search with K Nearest Neighbour Classifier
Grid Search with Support Vector Classifier
Grid Search with Decision Tree Classifier
Conclusion
__Introduction__
It is important that credit card companies are able to recognize fraudulent credit card transactions so that customers are not charged for items that they did not purchase. Eventually, it is also important for companies NOT to detect transactions which are genuine as fraudulent, otherwise, companies would keep blocking the credit card, and which may lead to customer dissatisfaction. So here are two important expects of this analysis:

What would happen when the company will not able to detect the fraudulent transaction and would not confirm from a customer about this recent transaction whether it was made by him/her.

In contract, what would happen when the company will detect a genuine transaction as fraudulent and keep calling customer for confirmation or might block the card.

The datasets contain transactions that have 492 frauds out of 284,807 transactions. So the dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions. When we try to build the prediction model with this kind of unbalanced dataset, then the model will be more inclined towards to detect new unseen transaction as genuine as our dataset contains about 99% genuine data.

As our dataset is highly imbalanced, so we shouldn't use accuracy score as a metric because it will be usually high and misleading, instead use we should focus on f1-score, precision/recall score or confusion matrix.

__Conclusion__¶
We were able to accurately identify fraudulent credit card transactions using a random forest model with oversampling technique. We, therefore, chose the random forest model with oversampling technique as the better model, which obtained recall score of 99% on the test set.

I hope I was able to explain my findings well and thanks so much for reading!

I welcome comments, suggestions, corrections and of course votes also
