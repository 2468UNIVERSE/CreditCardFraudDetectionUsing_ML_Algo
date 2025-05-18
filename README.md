
link for the dataset: https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud

1- Project Objective
The aim of this project is to build a machine learning model that can effectively detect fraudulent activities in a given dataset. Fraud detection is a critical application of machine learning, especially in sectors like banking, finance, and e-commerce. The model learns from historical data containing both fraudulent and non-fraudulent records and predicts whether a new transaction is likely to be fraudulent.

2- Algorithms Used
In this experiment, two classification algorithms were applied and compared:

Logistic Regression
A statistical model that uses a logistic function to model the probability of a binary outcome. It is widely used for binary classification problems like spam detection, disease prediction, and fraud detection.

Decision Tree Classifier
A tree-based model that splits the dataset into branches based on feature values, eventually leading to a decision outcome. It is intuitive, easy to visualize, and handles both numerical and categorical data effectively.

3- Why We Chose Decision Tree Classifier
After training both models on the dataset and evaluating their performance on unseen test data, the Decision Tree Classifier outperformed Logistic Regression across all key evaluation metrics:

Metric	    LogistiRegression	    Decision Tree
Accuracy	        94.54%	           99.82%
Precision	        97.44%	           99.75%
Recall	          91.49%	           99.90%
F1 Score	        94.36%	           99.82%

These results show that the Decision Tree Classifier is extremely effective at detecting fraud in this dataset with very high accuracy and recall. In fraud detection, recall is especially important, as it measures how well the model catches fraudulent cases (true positives). A higher recall means fewer frauds are missed.

4- Why Not Logistic Regression?
Although Logistic Regression is a solid baseline algorithm, it is less flexible in capturing complex patterns and interactions between features compared to Decision Trees. In this experiment, Logistic Regression achieved good performance but missed more fraudulent cases than the Decision Tree. In sensitive tasks like fraud detection, even a small number of false negatives (missed frauds) can be costly.

5- How This Model Helps in Fraud Detection
Using the trained Decision Tree Classifier, we can now:

Detect whether a given transaction or entry is likely to be fraudulent or legitimate.

Minimize financial losses by automating fraud detection with high accuracy.

Enable companies to take proactive action against suspicious activities in real-time.

This project serves as a foundation for building more advanced fraud detection systems that can incorporate real-time monitoring, anomaly detection, and ensemble models.

6- What's Inside this Project
Data Preprocessing and Feature Engineering

Model Training and Evaluation

Performance Metrics Comparison

Final Model Selection (Decision Tree Classifier)

Code and Notebooks for Reproducibility
