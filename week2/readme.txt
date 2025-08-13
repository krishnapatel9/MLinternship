Week 2: Model Mechanics, Validation & Tree-Based Methods 


1. How Models Work & Basic Data Exploration
Key Terminologies: 
Model Mechanics: Decision boundary (linear vs. non-linear), feature weights, probability calibration (logistic regression).  
Data Exploration: EDA (Exploratory Data Analysis), descriptive statistics (mean, median, skew), correlation heatmaps, missing value imputation (median/mode).  

What I Knew Before:
Basic Pandas operations (e.g., head(), describe()).  
Logistic regression as a binary classifier.  

What I Learned:  
Feature Importance: How coefficients in logistic regression indicate feature impact (e.g., Sex vs. Fare in Titanic survival).  
Visual EDA*: Used histograms (matplotlib) and correlation matrices to identify relationships (e.g., Pclass strongly correlates with Fare).  
Handling Missing Data*: Imputed Age with median to avoid bias.  

Description:
Performed EDA on Titanic data to identify key predictors (e.g., Sex, Pclass). Used visualizations to spot imbalances (e.g., more non-survivors in Pclass=3) and imputed missing values strategically.  


2. Model Validation & Evaluation  
Key Terminologies: 
Validation: Train-test split (test_size=0.2), cross-validation (cv=3 in GridSearchCV).  
Metrics: Precision/recall tradeoff (e.g., prioritizing recall for survival prediction), F1-score (harmonic mean), confusion matrix.  

What I Learned: 
Threshold Tuning: Adjusting decision thresholds to optimize for recall (minimizing false negatives in survival cases).  
Cross-Validation: Used GridSearchCV to validate hyperparameters (C=0.1 best for logistic regression).  



3. Underfitting vs. Overfitting & Regularization 
Key Terminologies:  
Underfitting: High bias (e.g., simplistic model with low max_iter).  
Overfitting: High variance (e.g., complex trees memorizing noise).  
Solutions: Regularization (C parameter in logistic regression), pruning (for trees).  


4. Random Forests & Feature Importance  
Key Terminologies:
Ensemble Methods: Bagging (Random Forest), boosting (Gradient Boosting).  
Feature Importance: Gini impurity reduction (how much a feature improves prediction).  


What I Learned:
Interpretability: Random Forests provide native feature importance (e.g., Sex most critical for survival).  
Hyperparameters: Tuned n_estimators (more trees reduce variance but increase compute).  


 5. Practical Implementation
Steps Followed:  
1. Preprocessing:  
    Encoded Sex (male=0, female=1), imputed Age/Fare.  
    Dropped high-cardinality columns (Ticket, Cabin).  
2. Modeling:  
    Logistic Regression (baseline: 81% accuracy).  
    Random Forest (improved to 83% with feature importance analysis).  
3. Documentation:  
    Saved as week2_titanic_classification.ipynb with clear markdown explanations.  

 
Tree-based models (Random Forests) outperformed logistic regression by capturing non-linear relationships, while EDA and validation ensured robustness.  

