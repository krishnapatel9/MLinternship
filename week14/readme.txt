Week 14 – Word Embeddings
What Are Word Embeddings?
Word embeddings are a method of representing words as dense numerical vectors.
Unlike one-hot vectors, which treat every word as independent, embeddings place words in a continuous vector space where:
Words with similar meanings are located closer together
Semantic relationships are preserved (e.g., king → queen, Paris → France)
They capture context, analogy relationships, and deeper linguistic patterns
These embeddings form the foundation for modern NLP models such as Word2Vec, GloVe, FastText, and transformer-based architectures.

Experiments Conducted
1. Exploring Word Similarities
We evaluated semantic similarity between words using pretrained Word2Vec embeddings.
Queries such as:
most similar to “king”
most similar to “queen”
relationships involving gender or roles
allowed us to observe how embeddings store meaning.

2. Visualizing Embeddings with t-SNE
A t-SNE dimensionality reduction was performed to project high-dimensional word vectors (300D) into a 2-dimensional space.
The words visualized included:
king, queen, prince, princess (royalty)
man, woman, child (gender/family roles)
This created a cluster map showing how semantically related words group together.

Key Observations
1. Semantic Clustering
Words with related meanings naturally grouped together:
“king” and “queen” appeared very close due to shared royal and gender characteristics.
“prince” and “princess” also formed their own sub-cluster within the royal group.

2. Gender & Role Separation
“man” and “woman” clustered together but at a reasonable distance from the royalty-related words.
“child” was placed slightly apart, reflecting a different semantic role but still connected through family-related proximity.

3. Preserved Relationships
The visualization highlights how embeddings capture:
Hierarchical relationships
Gender distinctions
Family/royalty groupings
Semantic proximity learned from large text corpora

📝 Summary
This exercise demonstrates how pretrained word embeddings:
Convert words into meaningful vector representations
Maintain semantic structure
Enable similarity queries and analogy reasoning
Allow visual understanding of word relationships through t-SNE
This documentation forms the conceptual and experimental overview for Week 14’s work on word embedding
