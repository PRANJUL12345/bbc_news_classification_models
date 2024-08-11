# bbc_news_classification_models
The purpose of this model is to perform text classification on BBC news articles.  Specifically, it aims to automatically categorize news articles into one of five categories:  
1. Business
2. Entertainment
3. Politics 
4. Sports 
5. Technology

The main goals of this text classification model are :

1. Automated Categorization: To automatically assign a category to a given news article based on its content. 
This can be useful for organizing large amounts of news data efficiently.

2. Content Analysis: To understand the key features or words that distinguish different categories of news articles.

3. Information Retrieval: To help in quickly finding articles related to a specific category.

4. Demonstration of NLP Techniques: To showcase various Natural Language Processing (NLP) techniques such as text preprocessing, 
vectorization (TF-IDF), 
and different machine learning algorithms for classification.

5. Performance Comparison: To compare the effectiveness of different machine learning algorithms 
(Logistic Regression, Random Forest, and K-Nearest Neighbors) for this specific text classification task.

6. Scalability Testing: To explore how well these techniques work on a real-world dataset and consider potential challenges in scaling to larger datasets.

The model processes the text data, converts it into a numerical format (using TF-IDF), 
and then uses machine learning algorithms to learn patterns that distinguish between the different categories. 
Once trained, the model can be used to predict the category of new, unseen news articles.

This type of model has practical applications in news aggregation services, content recommendation systems, 
or any platform that deals with large volumes of textual data and needs to organize or filter it by topic.




##################################################################################################################


# CONCLUSION
# The three model approaches
# Random Forest Model

# Pros

# -As the data is less this model will outperform all the other models providing a accuracy of 96.17%.
# -The predictive performance can compete with the best supervised learning algorithms.

# Cons

# -An ensemble model is inherently less interpretable than an individual decision tree.
# -Training a large number of deep trees can have high computational costs (but can be parallelized) and use a lot of memory.


# Logistic Regression

# Pros

# -It is easy to understand and it can also be trained on small dataset.

# Cons

# -The model is highly scalable although it is giving a accuracy of just 66.51%


# KNN Classification

# Pros

# -Simple algorithm — to explain and understand/interpret.
# -High accuracy (relatively) — it is pretty high but not competitive in comparison to better supervised learning models.It is providing a accuracy of 76.85% .


# Cons

# -Computationally expensive — because the algorithm stores all of the training data so it takes a lot of time to predict(not train).

# Challenges and Future Works

# -The regular expression approach for replacing specific keywords may not work as the data will increase, the cleaning will take more time and regex is not that much scalable. Even for 1 million records it will take days to process it and if it fails we cannot track it properly.
# -Preparation of the dataframe from the documents should be done properly to ensure no wrong labels.
# -If the size of the dataset increases then tf-idf method for vectorization will fail because of large matrix size.
# -Applying K-Fold Cross Validation on the data to find optimum value of K was computationally very intensive because of such large number of features.
# -Model training can be improved by trying other approaches which are build majorly for text classification and response is fast with a probability of each class label.
# -If the size increases and tf-idf starts to fail we can use tokenizer with CNN or Word Embedding with CNN


