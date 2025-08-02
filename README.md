Machine Learning Concepts & Key Terminologies Explored
1. Linear & Logistic Regression
Key Terminologies:
Linear Regression: Continuous prediction, MSE (Mean Squared Error), Gradient Descent, Hyperparameters (learning rate, epochs), Feature Scaling.
Logistic Regression: Sigmoid function, Binary/Multi-class classification, Cross-Entropy Loss, Decision Boundary, Regularization (L1/L2), Odds Ratio.

What I Knew Before:
Basic idea of fitting a line to data (linear regression).
Logistic regression as a binary classifier (sigmoid curve).

What I Learned:
Mathematics: How gradient descent minimizes MSE (linear) and cross-entropy loss (logistic).
Regularization: L1/L2 penalties to control overfitting.
Probability Calibration: Interpreting logistic outputs as probabilities.

Challenges:
Debugging convergence issues in gradient descent (learning rate too high/low).
Choosing between L1 (sparsity) vs. L2 (smooth weights) regularization.

2. Classification Metrics & Model Evaluation
Key Terminologies:
Confusion Matrix: TP (True Positive), TN (True Negative), FP (False Positive), FN (False Negative).
Metrics: Accuracy, Precision, Recall, F1-Score, ROC Curve, AUC (Area Under Curve), Precision-Recall Tradeoff.
Bias-Variance Tradeoff, Imbalanced Data (oversampling/undersampling), Threshold Tuning.

What I Knew Before:
Accuracy as a simple metric.
Confusion matrix structure (TP, TN, FP, FN).

What I Learned:
Precision-Recall Tradeoff: Optimizing for false positives (precision) vs. false negatives (recall).
ROC/AUC: Visualizing model performance across thresholds.
Imbalanced Data: Techniques like SMOTE and class weighting

Description:
Dived into evaluating classifiers using metrics like precision (minimizing false positives) and recall (capturing all positives).
Analyzed ROC curves to compare models and addressed challenges like imbalanced datasets using resampling techniques.
Learned how adjusting decision thresholds impacts model performance in real-world scenarios.

3. Data Preprocessing & Feature Engineering
Key Terminologies:
Numerical Data: Normalization (Min-Max, Z-Score), Binning, Outlier Handling (IQR, Z-Score), Polynomial Features.
Categorical Data: One-Hot Encoding, Label Encoding, Target Encoding, Embeddings, Feature Crosses.
Feature Selection: Correlation Analysis, RFE (Recursive Feature Elimination), PCA (Dimensionality Reduction).

What I Knew Before:
Basic normalization (scaling 0–1).
One-hot encoding for categories.

What I Learned:
Advanced Techniques: Feature crosses (e.g., latitude × longitude for geospatial models).
Embeddings: Efficiently encoding high-cardinality categories.
Binning Strategies: Quantile vs. fixed-width for numerical data.

Description:
Mastered transforming raw data into model-ready features—scaling numerical data (normalization), encoding categories (one-hot for low cardinality, embeddings for high), 
and creating interaction terms (feature crosses). Practiced dimensionality reduction (PCA) and outlier detection to improve model robustness.

4. Generalization, Overfitting & Regularization
Key Terminologies:
Overfitting/Underfitting, Train-Validation-Test Split, Cross-Validation (k-Fold).
Regularization: L1 (Lasso), L2 (Ridge), Dropout (in NNs), Early Stopping.
Loss Curves: Training vs. Validation Loss, Learning Curves, Model Complexity Analysis.

What I Knew Before:
Overfitting = model memorizes training data.
Train-test splits as a simple solution.

What I Learned:
Diagnostics: Using validation loss curves to detect overfitting.
Regularization: How L2 shrinks weights and dropout works in NNs.
Early Stopping: Halting training when validation performance plateaus.

Challenges:
Tuning L2 hyperparameter (λ) without exhaustive search.
Explaining bias-variance tradeoff intuitively.

Description:
Investigated why models fail to generalize—overfitting (high variance) vs. underfitting (high bias). 
Implemented techniques like L2 regularization to penalize large weights and used cross-validation to ensure reliable performance.
Analyzed loss curves to diagnose issues and optimized model complexity.
