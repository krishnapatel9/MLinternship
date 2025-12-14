Week 17- Data Cleaning & Exploratory Data Analysis (EDA)

Exploratory Data Analysis (EDA) is a foundational skill in data science, as real-world datasets are often incomplete, inconsistent, and noisy.

🎯 Objectives
Understand the structure and quality of the dataset
Identify and handle missing or inconsistent data
Analyze feature distributions and relationships
Detect outliers and anomalies
Extract insights that influence future modeling decisions

📂 Dataset Description
The dataset contains house sales information including:
Property characteristics (bedrooms, bathrooms, square footage)
Location details (latitude, longitude, waterfront)
Construction quality and condition
Target variable: house price
Each row represents a single house sale, and columns represent property attributes.

🔍 1. Data Inspection
Before any analysis, the dataset is inspected to understand:
Number of rows and columns
Data types (numerical vs categorical)
Presence of missing or null values
Basic statistical properties such as mean, median, and range
This step helps identify data quality issues early.

🧹 2. Data Cleaning Strategy
Missing Data Handling
Real-world datasets often have missing values due to:
Data collection errors
Optional or unavailable information
The following strategies are applied:
Columns with excessive missing values are removed to avoid unreliable analysis
Numerical features are imputed using median values to reduce outlier influence
Categorical features are filled using the most frequent category (mode)
This ensures the dataset remains complete and usable.

📊 3. Univariate Analysis
Univariate analysis focuses on individual features to understand:
Distribution shape (normal, skewed)
Spread and central tendency
Presence of extreme values
Target Variable (Price)
House prices are typically right-skewed
Log transformation is applied to normalize the distribution
Normalized distributions improve statistical analysis and model performance

🔗 4. Bivariate Analysis
Bivariate analysis examines relationships between two variables, especially:
Feature vs target relationships
How individual attributes influence house prices
Key observations include:
Larger living areas generally correspond to higher prices
Higher number of bathrooms indicates premium housing
Construction quality has a strong impact on price
This step helps identify important predictive features.

🔥 5. Correlation Analysis
Correlation analysis measures linear relationships between numerical features.
Strong positive correlations highlight influential variables
Weak or negative correlations indicate limited impact
Highly correlated features help in feature selection
Understanding correlations prevents:
Redundant features
Multicollinearity in models

⚠️ 6. Outlier Detection
Outliers are extreme values that can distort analysis.
Housing data naturally contains high-value properties
Interquartile Range (IQR) method is used to detect anomalies
Outliers are analyzed rather than blindly removed
Outlier detection ensures robust modeling decisions.

🧠 Key Insights
Living area (sqft_living) is one of the strongest price drivers
Location features significantly influence property value
Quality and condition outperform simple room counts
Log-transformed prices yield more stable analysis

📈 Why EDA Matters
Exploratory Data Analysis:
Reduces risk of incorrect assumptions
Improves model accuracy
Guides feature engineering
Builds intuition about real-world data

EDA is not optional — it is the backbone of data science workflows.
