This project applies K-Means clustering to segment customers based on their characteristics.
It is a full end-to-end unsupervised machine learning workflow, ideal for understanding customer behavior, market segmentation, and personalized targeting.

The dataset used is the Mall Customers Dataset, which contains basic demographic and spending information for mall customers.

Project Objectives

Perform clustering using K-Means

Automatically find the best number of clusters using the Elbow Method

Evaluate cluster quality using the Silhouette Score

Visualize clusters in 2D and 3D

Generate meaningful customer segment insights

Produce interpretable summaries for each cluster

Dataset

Dataset link:
Mall Customers Dataset – Kaggle
https://www.kaggle.com/datasets/shwetabh123/mall-customers

The dataset includes:

CustomerID

Gender

Age

Annual Income (k$)

Spending Score (1–100)

 Technologies Used

Python

Pandas

NumPy

Scikit-Learn (KMeans, StandardScaler, silhouette score)

Matplotlib

Seaborn

Plotly (optional for 3D interactive plots)

 Project Steps
1. Data Loading & Exploration

Load dataset

Check datatypes, missing values, and summary statistics

Visualize basic distributions like Income vs Spending Score

2. Feature Selection

Most relevant features for clustering:

Age

Annual Income (k$)

Spending Score (1-100)

3. Data Scaling

K-Means relies on Euclidean distance, so data is scaled using StandardScaler.

4. Finding Optimal K

Use the Elbow Method:

Train K-means with K from 1 → 10

Plot inertia (within-cluster variance)

Select K at the "elbow" point

5. Model Training

Fit K-Means with the chosen K and assign cluster labels.

6. Evaluation

Use Silhouette Score to measure:

Cluster separation

Cluster cohesion

A score >0.5 is considered good.
