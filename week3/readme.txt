Week-3 
1. Handling Missing Values
Key Terminologies:
Missing Value Approaches: Dropping columns, imputation (median/mode), extended imputation.
Imputation: Replacing missing values with a substitute, such as the mean, median, or mode.

What I Knew Before:
Drop Missing Values: The simplest method, but can lead to significant data loss if many values are missing.
Imputation: A better approach that preserves data. For example, using the median for numerical data prevents bias from outliers.

What I Learned:
Extended Imputation: More advanced methods like using machine learning models (e.g., K-Nearest Neighbors) to predict missing values based on
other features.

Description:
I learned three main strategies for handling missing data. The simplest is to drop rows or columns, but this can be wasteful. 
A more robust method is imputation, where missing values are replaced with a calculated value like the median or mode.
I also learned about more sophisticated techniques for complex datasets.

2. Categorical Variables
Key Terminologies:
Categorical Variables: Features with a limited number of distinct values (e.g., 'Color', 'City').
Encoding: Converting categorical data into a numerical format for machine learning models.
Encoding Approaches: Dropping variables, ordinal encoding, one-hot encoding.

What I Knew Before:
Drop Categorical Variables: Similar to dropping missing values, this is the easiest but often least effective approach.

What I Learned:
Ordinal Encoding: Assigning a numerical rank to categories based on their order (e.g., 'Small' = 1, 'Medium' = 2, 'Large' = 3).
One-Hot Encoding: Creating a new binary column for each category. This is ideal for nominal (unordered) data to prevent the model from 
misinterpreting a false sense of order.

Description:
I discovered three ways to prepare categorical data for modeling. The first is to drop them, which is often not ideal.
The other two methods, ordinal and one-hot encoding, convert categories into numbers. 
One-hot encoding is particularly useful for nominal data to avoid a false sense of hierarchy, which could confuse a model.

3. Pipelines
Key Terminologies:
Pipeline: A tool for bundling data preprocessing and modeling steps into a single object.
Preprocessing: Steps taken to prepare data before modeling.
Modeling: The process of training a machine learning model.

What I Knew Before:
I was familiar with individual data preprocessing steps.

What I Learned:
Step 1: Define Preprocessing Steps: I learned how to define the specific transformations needed, like imputation and encoding.
Step 2: Define the Model: I learned how to specify the machine learning algorithm to be used within the pipeline.
Step 3: Create and Evaluate the Pipeline: I learned to combine these steps into a single pipeline object and evaluate its performance.

Description:
Pipelines streamline the machine learning workflow by packaging preprocessing and modeling steps together. This simplifies the code, 
making it more organized and reproducible. It's a best practice for managing a series of steps as if they were one single operation.

4. Cross-Validation
Key Terminologies:
Cross-Validation: A technique for assessing a model's performance by training and testing on different subsets of the data.
Folds: The number of data partitions used in cross-validation.
cross_val_score(): A scikit-learn function to perform cross-validation.

What I Knew Before:
I was familiar with the basic train-test split method for model validation.

What I Learned:
When to use Cross-Validation: It's used when a simple train-test split may not be reliable, especially with smaller datasets,
to get a more robust estimate of model performance.cv Parameter: This parameter in cross_val_score() controls the number of folds, or
data partitions, to be created for the validation process.

Description:
Cross-validation is a more robust way to evaluate a model's performance than a simple train-test split. Instead of a single split,
it divides the data into multiple "folds." The model is trained on a subset of the folds and tested on the remaining one. 
This process is repeated, and the results are averaged to give a more reliable performance score.

5. XGBoost
Key Terminologies:
XGBoost: An optimized gradient boosting library.
Gradient Boosting: An ensemble method that builds a series of weak models (decision trees) sequentially, where each new model corrects the
                   errors of the previous one.
Parameter Tuning: Adjusting model settings to optimize performance.
Parameters: Key settings like n_estimators, early_stopping_rounds, n_jobs, and learning_rate.

What I Knew Before:
I had a basic understanding of decision trees.

What I Learned:
Ensemble Method: XGBoost is a type of gradient boosting, which combines multiple simple models to create a more powerful one.
Parameter Tuning: I learned how to tune key parameters:
                  n_estimators: The number of trees in the model.
                  early_stopping_rounds: Stops training early if validation performance doesn't improve, preventing overfitting.
                  n_jobs: The number of CPU cores to use for training, for faster processing.
                  learning_rate: The "step size" at each iteration, which controls how much each new tree contributes to the final prediction.
Description:
XGBoost is a highly efficient and powerful ensemble method that uses gradient boosting. It builds a series of decision trees sequentially,
with each new tree trying to fix the mistakes of the previous ones. I learned about several key parameters to tune the model's performance,
such as the number of trees and the learning rate.
