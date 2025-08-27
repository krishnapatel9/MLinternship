1.Introduction to Feature Engineering
Key Terminologies:
Feature Engineering: Process of creating new input features or modifying existing ones to improve model performance.
Feature Transformation: Changing the format, scale, or values of features.
Feature Selection: Identifying the most relevant features for a model.

Description:
I understood that feature engineering is a crucial step in the ML pipeline. 
It involves creating, transforming, or selecting features that allow models to perform better. 
A well-engineered feature set can turn a simple model into a highly effective one.

2.Mutual Information
Key Terminologies:
Mutual Information (MI): A measure of dependency between two variables.
Feature Relevance: Identifying how much information a feature provides about the target.

What I Knew Before:
Correlation measures linear relationships.
Feature importance can be measured using model-based methods (e.g., tree-based).
MI can capture both linear and nonlinear relationships.
Unlike correlation, MI works well even when the relationship is not straight-line dependent.

Description:
I learned that mutual information helps identify the most useful features by checking how much they reduce uncertainty about the target.
It’s especially powerful when relationships are nonlinear, where traditional correlation might fail.

3.Creating Features
Key Terminologies:
Feature Creation: Building new features from existing ones.
Feature Transformation: Using mathematical or domain-specific rules to derive new features.
Pandas Feature Engineering: Leveraging pandas for operations like aggregation, binning, or extracting datetime components.

What I Knew Before:
New features can be made by combining columns (e.g., ratio of two features).
Datetime features like day, month, and weekday are often useful.

Description:
I learned how to construct new features that highlight important aspects of the data.
Using pandas transformations, it’s possible to enrich datasets by extracting more meaningful signals for machine learning models.

4.Principal Component Analysis (PCA)
Key Terminologies:
PCA: A dimensionality reduction technique that transforms features into uncorrelated components.
Variance Explained: The amount of information captured by each principal component.
Dimensionality Reduction: Reducing the number of input features while preserving most of the information.

What I Knew Before:
PCA reduces dimensions by projecting data into new axes.
It helps simplify models and reduce overfitting.

Description:
I learned that PCA is not only a dimensionality reduction tool but also a way to generate new, independent features. 
These transformed features can highlight variation in the data and improve model stability.

5.Target Encoding
Key Terminologies:
Target Encoding: Encoding categorical variables using the mean of the target variable for each category.
Categorical Feature Transformation: Converting categories into numerical representations.
Data Leakage: Risk of using information from the target incorrectly.

What I Knew Before:
One-hot encoding is a common method for handling categorical features.
Label encoding assigns integer values but may impose false ordinal relationships.

What I Learned:
Target encoding provides a more compact representation of categorical variables.
It is especially useful for high-cardinality categorical features.
Care must be taken to avoid leakage (e.g., using cross-validation encoding).

Description:
I understood that target encoding is a powerful method for categorical features, especially when categories are many. 
It creates meaningful numeric values that capture target patterns, but requires careful implementation to prevent leakage.
