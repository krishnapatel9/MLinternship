Week 11: Data Augmentation  

Real-world datasets are often limited or imbalanced.  
Data augmentation artificially increases dataset diversity, enabling models to learn invariant features (e.g., rotation, lighting, or scale changes) and
perform better on unseen data.  

Implementation Overview  
Dataset: CIFAR-10 (32 × 32 RGB images)  
Augmentations Applied: Horizontal flip, random rotation, brightness/contrast adjustment, random scaling  
Model Used: Convolutional Neural Network (CNN)  
Comparison: Model trained on original data vs. augmented data  


Results Summary  
 Dataset Type   | Accuracy (%) 
 Original Data  | 68.45 
 Augmented Data | 73.90 

Data augmentation improved accuracy by roughly 5%, showing better model generalization and reduced overfitting.

Visual Examples  
 Original Image      | Augmented Version 
 insert sample image | insert augmented sample

Observations:
- Data augmentation is an essential step to build robust and accurate AI/ML models.  
- It reduces overfitting and improves model generalization across unseen data.  
- Even simple transformations can provide measurable accuracy gains.  
