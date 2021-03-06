# sklearn-cluster-wine-reviews
Term frequency, vectorization, and clustering of Wine Reviews

Using wine review data from Kaggle, I subsetted to reviews having points 95 or higher. A term frequency - inverse document frequency 
(tf-idf) matrix is constructed.  Then, a cosine similarity matrix is constructed as 1-cosine_similarity(tfidf_matrix), which is later 
used for Multi-Dimensional-Scaling before visualization.  Sklearn k-means is used for clustering based on the tfidf_matrix. Attempting different number of clusters yields similar results - most wine reviews are not very unique and use very common language across documents.

![scatter](https://github.com/datavizhokie/sklearn-cluster-wine-reviews/blob/master/3-cluster%20scatter.PNG "3-cluster scatter")
