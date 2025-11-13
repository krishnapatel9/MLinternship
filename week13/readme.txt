This project implements a complete Natural Language Processing (NLP) pipeline for SMS spam classification using classical machine learning techniques. 
The implementation demonstrates the entire workflow from raw text preprocessing to model training and evaluation.
# Preprocessing Pipeline
1. Text Cleaning
   - Lowercasing all text
   - Removal of special characters and numbers
   - Handling of missing values

2. Tokenization & Normalization
   - Word tokenization using NLTK
   - Parts-of-Speech (POS) tagging for contextual lemmatization
   - Stopword removal using NLTK's English stopwords corpus
   - Lemmatization with WordNetLemmatizer

3. Feature Engineering
   - N-gram analysis (unigrams and bigrams)
   - Feature selection based on term frequency

# Vectorization Methods
- Count Vectorization: Convert text to word frequency vectors
- TF-IDF Vectorization: Term Frequency-Inverse Document Frequency for better feature weighting
- Feature Dimension: 3,000 most important features

# Machine Learning Models
Three classical algorithms were implemented and compared:
1. Logistic Regression - Linear classification model with probability estimates
2. Multinomial Naive Bayes - Probabilistic classifier based on Bayes theorem
3. Random Forest Classifier - Ensemble method with multiple decision trees

# Results & Performance
# Model Evaluation
- Train-Test Split: 80-20 stratified split
- Evaluation Metrics: Accuracy, Precision, Recall, F1-Score
- Cross-validation: Used for robust performance estimation

# Key Findings
- TF-IDF vectorization consistently outperformed simple count vectorization
- Proper text preprocessing significantly improved model accuracy
- The best performing model achieved strong classification performance
- Feature importance analysis provided interpretable insights into spam detection patterns

# Business Impact
This implementation demonstrates a production-ready spam detection system that can:
- Automatically classify SMS messages as spam or legitimate
- Provide interpretable results for transparency
- Scale to handle large volumes of text data
- Serve as a foundation for more advanced NLP applications

#Technical Stack
- Programming Language: Python 3.x
- Libraries: 
  - Core: pandas, numpy
  - NLP: NLTK
  - Machine Learning: scikit-learn
  - Visualization: matplotlib, seaborn
- Tools: Jupyter Notebook

#Learnings
- Mastered the complete NLP pipeline from raw text to deployed model
- Understood the critical importance of proper text preprocessing
- Gained practical experience with multiple vectorization techniques
- Learned to compare and evaluate different machine learning algorithms
- Developed skills in model interpretation and feature importance analysis
