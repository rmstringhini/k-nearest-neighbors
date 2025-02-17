The KNN (K-Nearest Neighbors) algorithm is a simple yet effective supervised learning algorithm used for classification and regression tasks. It is non-parametric and instance-based, meaning that it does not assume an underlying data distribution and makes predictions based on the similarity of new data points stored training examples.

The KNN algorithm works by identifying a specified number of training samples that are closest to a new data point and using their labels to make a prediction.

How KNN works:

1) Choose the number of neighbors (K):
   - The user selects a integer K, which determines how many nearest neighbors will be used to classify or predict the new data point;
   - A small K makes the model sensitive to noise, while a large K smooths the decision boundary but may lead to misclassification;

2) Compute the distances between the new data point and all training points:
   - Euclidean distance: $d(p,q)=\sqrt{\sum_{i=1}^{n}(p_i - q_i)^2}$
   - Manhattan distance: $d(p,q)=\sum_{i=1}^{n}\left | p_i - q_i\right |$
   - Minkowski distance: $d(p,q)=\left ( \sum_{i=1}^{n}\left | p_i - q_i\right |^p \right )^\frac{1}{P}$, with _p_ determining the type of distance (1 -> manhattan / 2 -> euclidean)

4) Find the K nearest neighbor:
   - Sort the training points based on their distance from the query point.
   - Select the K closest points (K nearest neighbors)

5) Make a prediction based on the majority vote (for classification) or average (for regression):
   - For classification: the label with the most occurences among the K neighbors is assigned to the new data point
   - For regression: the predicted value is the average of the K neighbor's values


![KNN](https://github.com/user-attachments/assets/13169495-a746-4d80-9bf6-ee2d5cd576c3)
