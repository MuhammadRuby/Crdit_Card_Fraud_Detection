
# Credit Card Fraud Detection with Machine Learning

This repository contains the code for a credit card fraud detection system using machine learning techniques. The project is designed to help identify fraudulent transactions in real-time, minimizing financial losses and protecting consumers.

## Goal
We aim to build a model to detect if a transaction is normal or fraudulent using machine learning techniques.

## Structure of project
1. Importing Libraries
    - Pandas & NumPy: For data manipulation.
    - Matplotlib & Seaborn: For visualization.
    - Scikit-learn: For model building (Logistic Regression, Decision    Tree,  Random Forest) and performance metrics.
    - Imbalanced-learn (SMOTE): To handle imbalanced datasets.
    - Joblib: For model serialization.
2. Loading and Exploring the Dataset
    - Data Source: The dataset is available on Kaggle, containing  details of transactions labeled as normal or fraudulent.
    - Data Cleaning:
     * Duplicate data is removed.
     * Null values are confirmed as absent.
3. Data Visualization
    - Histograms and box plots are used to understand the distribution of transaction amounts.
    - Count plot displays the distribution between fraudulent and  non-fraudulent transactions.
4. Handling Class Imbalance
    - The dataset has a class imbalance, with far fewer fraudulent transactions.
    - Class Imbalance Handling:
        * Undersampling: Reducing the majority class size.
        * SMOTE: Synthetic data generation for the minority class.

5. Feature Engineering
    - The Amount column is standardized to match the range of other features.
    - The Time column is dropped as it's irrelevant to the classification task.
6. Model Selection
- Three models are evaluated:
    * Logistic Regression
    * Decision Tree
    * Random Forest
- Performance metrics include:
    * Accuracy: Percentage of correct predictions.
    * Precision: How many selected items are relevant.
    * Recall: How many relevant items are selected.
    * F1-Score: Harmonic mean of precision and recall.
    * Confusion Matrix: Evaluates true positives, true negatives, false positives, and false negatives.
7. Final Model - Random Forest
    - Random Forest achieved the best performance with an accuracy of 99.99%.
    - The model is saved as CerditCardRandomForestModel.pkl using joblib for later use.
8. Deploying the Model
    - The trained Random Forest model can be loaded and tested on new data to predict if a transaction is fraudulent.
# Conclusion
  - Random Forest is chosen as the final model due to its superior accuracy, recall, and precision.
  - This solution is highly applicable in real-world settings like fraud detection where minimizing both false positives and negatives is critical.

# Links 
- [Kaggle Notebook](https://www.kaggle.com/code/muhammadrubymuhammad/creditcardfrauddetection?scriptVersionId=199660855)
- [LinkedIn Account](https://www.linkedin.com/in/muhammad-ruby-muhammad)
- [Email](mohamedroby831@gmail.com)

## how to run project >>


1. Clone the repository:

        git clone https://github.com/MuhammadRuby/Crdit_Card_Fraud_Detection.git 

2. Install dependencies:

        python -m venv venv
        
        source venv/bin/activate  # For Linux/macOS
        
        venv\Scripts\activate.bat  # For Windows
        
        pip install -r requirements.txt

3. download data set from this Link [Kaggle Dataset Link](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud)
4. edit path of data in code and run 


## Author
Muhammad Ruby

