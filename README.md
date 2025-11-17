# 🛍️ Mall Customer Segmentation using K-Means Clustering

## Introduction
This project demonstrates how to perform customer segmentation using the K-Means clustering algorithm. By analyzing customer data, we can group similar customers into distinct segments, allowing businesses to tailor marketing strategies and improve customer experience.

## What is K-Means Clustering?
Imagine you have a big pile of different colored candies, but they're all mixed up. K-Means clustering is like a robot that helps you sort them into separate piles based on their colors. 

In more technical terms, K-Means is an **unsupervised machine learning algorithm** that partitions `n` observations into `k` clusters. Each observation belongs to the cluster with the nearest mean, serving as a prototype of the cluster.

**How it works (in simple steps):**
1.  **Choose K**: You decide how many 'piles' (clusters) you want to make.
2.  **Random Start**: The robot randomly picks `K` spots on the floor to start the 'piles'. These are called **centroids**.
3.  **Assign**: Each candy goes to the closest pile (centroid).
4.  **Adjust**: Once all candies are assigned, the robot recalculates the center of each pile (the new centroid).
5.  **Repeat**: Steps 3 and 4 are repeated until the piles stop changing much, meaning the candies are sorted as best as they can be.

## Example: Customer Segmentation
In this notebook, we apply K-Means clustering to a dataset of mall customers. The goal is to segment customers based on their `Annual Income` and `Spending Score`. This helps the mall understand different customer behaviors and preferences.

**The process involves:**
1.  **Data Loading**: Importing the `mall_visitors.csv` dataset.
2.  **Exploratory Data Analysis (EDA)**: Visualizing distributions and relationships between features like Age, Annual Income, and Spending Score.
3.  **Feature Selection & Scaling**: Using `AnnualIncome` and `SpendingScore` as features and scaling them to ensure all features contribute equally to the clustering.
4.  **Determining Optimal K**: Using the Elbow Method and Silhouette Score to find the best number of clusters.
5.  **K-Means Application**: Running the K-Means algorithm with the optimal `K`.
6.  **Segment Profiling**: Analyzing the characteristics of each customer segment (e.g., "High Spenders," "Low Spenders," "Medium Spenders").
7.  **Visualization**: Creating plots to visualize the clusters and their distributions.
8.  **Prediction Tool**: A simple interactive tool to predict the segment of a new customer.

## Data
The dataset used contains information about mall customers, including:
*   `CustomerID`
*   `Age`
*   `AnnualIncome` (in k$)
*   `SpendingScore` (1-100)

## Key Results (Customer Segments)
Based on the analysis, we identified three main customer segments:

*   **Low Spenders**: Customers with moderate to high annual income but low spending scores.
*   **Medium Spenders**: Customers with high annual income and high spending scores.
*   **High Spenders**: Customers with lower annual income but high spending scores.

These segments can be used to develop targeted marketing campaigns, personalized offers, and optimize store layouts.

## How to Run
1.  **Upload `mall_visitors.csv`**: Ensure the dataset is uploaded to your Colab environment or provide the correct path.
2.  **Run All Cells**: Execute all code cells in the notebook sequentially.
3.  **Interact**: Use the provided interactive prediction tool to test new customer profiles.

This project provides a practical application of K-Means clustering for real-world business problems
