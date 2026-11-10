# Feature-Reduction

Breast Cancer Classification with Feature Selection

This repository implements a machine learning pipeline to classify breast tumors as either malignant or benign using the Breast Cancer Dataset. 

It demonstrates a robust approach from exploratory data analysis to feature selection and classification.  
Abstract Accurate diagnosis of breast cancer is crucial for successful treatment and patient survival. 
This project leverages machine learning to automate the classification of tumor samples based on fine-needle aspirate (FNA) image features. 

To optimize model efficiency and generalizability, SelectKBest (using the ANOVA F-value method) is employed to extract the top 10 most statistically significant features from a 30-feature dataset, reducing dimensionality while preserving predictive power. 

A Logistic Regression model is trained on these selected features. This lightweight pipeline aims to provide a rapid, interpretable, and computationally efficient diagnostic tool.  

*Project Workflow*  
-  Exploratory Data Analysis (EDA): Inspected data distribution, checked for missing values, and visualized outliers using boxplots.
-  Data Splitting: Partitioned the dataset into training (80%) and testing (20%) sets using stratified splitting to preserve class balance.
-  Feature Selection: Utilized SelectKBest with the f_classif score function to select the top 10 features, filtering out noisy and redundant dimensions.
-  Model Training: Fit a Logistic Regression classifier on the reduced feature space.
-  Evaluation: Evaluated performance using key classification metrics including Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix to understand prediction behavior.
