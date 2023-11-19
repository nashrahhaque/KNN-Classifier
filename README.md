# KNN-Classifier



This Python code demonstrates the use of the K-Nearest Neighbors (KNN) classification algorithm to classify data based on the distance to its k-nearest neighbors as asked in homework 2. The code loads datasets, performs classification, and reports test accuracies.

Dependencies:
- `numpy` for numerical operations - `pandas` for data manipulation
- `collections` for counting elements
  
Code Overview:
1. **Loading the Datasets**: The code reads two CSV files, `spam_train.csv` and `spam_test.csv`, and extracts features and labels.
2. **Euclidean Distance Calculation**: It defines a function `euclidean_distance` to calculate the Euclidean distance between two data points.

 3. **K-Nearest Neighbors Classification**: The `k_nearest_neighbors` function is used for classification. It computes distances between a test point and all training data, finds the k-nearest neighbors, and selects the most common label among them.
4. **Testing with Different k Values**:
- Part (a): The code tests the KNN classifier without normalization for different values of k. It
reports the accuracy for each k.
- Part (b): The code normalizes features using Z-score and tests the KNN classifier for the same
set of k values, reporting the accuracies.
5. **Generating Predicted Labels for First 50 Instances (Part c)**:
- The code generates predicted labels for the first 50 instances from the test data.
- It performs this prediction for each value of k from `k_values_c` and displays the results as
predicted labels for each instance.

Usage:
1. Ensure the `spam_train.csv` and `spam_test.csv` files are in the same directory as this script. 2. Run the code using a Python interpreter.
3. The code will print test accuracies for different values of k, both with and without Z-score normalization.
4. The code will also generate predicted labels for the first 50 instances for each k in `k_values_c`.
