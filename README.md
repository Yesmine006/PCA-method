# PCA-method

The Principal Component Analysis is a popular unsupervised learning technique for reducing the dimensionality of data. It increases interpretability yet, at the same time, it minimizes information loss. It helps to find the most significant features in a dataset and makes the data easy for plotting in 2D and 3D.

Goal of PCA:
• Find a new basis to re-express a dataset
This new basis should
  1) filter out noise,
  2) reveal interesting structure

Solution:
Find a linear transformation matrix P such that Y=PX and the covariance matrix of Y (CY) is a diagonal matrix. To do that we need to follow the following steps:
  1. Organize data into an m x n matrix X
• m: number of measurement types (feature vector size)
• n: number of samples
  2. Compute data (sample) mean vector
  3. Subtract off mean vector from dataset
  4. Calculate sample covariance matrix CX
  5. Calculate eigenvectors of matrix CX à obtain matrix P
  6. Apply change of base
  End - Y is the transformed data matrix

In this notebook we will be testing the PCA (Principal components) method.
1. First we will upload the MNIST dataset which is a large collection of handwritten digits. It is a very popular dataset in the field of image processing. It is often used for benchmarking machine learning algorithms.

2. We will compute the PCA method (steps are mentioned in the notebook)
