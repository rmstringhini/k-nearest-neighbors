The KNN (K-Nearest Neighbors) algorithm is a simple yet effective supervised learning algorithm used for classification and regression tasks. It is non-parametric and instance-based, meaning that it does not assume an underlying data distribution and makes predictions based on the similarity of new data points stored training examples.

The KNN algorithm works by identifying a specified number of training samples that are closest to a new data point and using their labels to make a prediction.

How KNN works:

1) Choose the number of neighbors (K):
   - The user selects a integer K, which determines how many nearest neighbors will be used to classify or predict the new data point;
   - A small K makes the model sensitive to noise, while a large K smooths the decision boundary but may lead to misclassification;

2) Compute the distances between the new data point and all training points:
   - The most common distance metric used is Euclidean distance, but other options include:
       - Manhattan distance
       - Minkowski distance
       - Cosine similarity

3) Find the K nearest neighbor:
   - Sort the training points based on their distance from the query point.
   - Select the K closest points (K nearest neighbors)

4) Make a prediction based on the majority vote (for classification) or average (for regression):
   - For classification: the label with the most occurences among the K neighbors is assigned to the new data point
   - For regression: the predicted value is the average of the K neighbor's values


![KNN](https://github.com/user-attachments/assets/13169495-a746-4d80-9bf6-ee2d5cd576c3)
