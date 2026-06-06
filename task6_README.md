# synent-task6-customersegmentation-yourname

## Problem Statement

A mall wants to understand its customers better so it can target different groups with the right offers. Since there are no predefined labels, the task was to use clustering to group customers based on their income and spending behavior.

## Dataset Details

- Dataset: Mall Customer Segmentation Dataset
- Source: Kaggle
- Contains 200 customer records with age, gender, annual income, and a spending score assigned by the mall.
- Format: CSV

## Approach

I selected annual income and spending score as the two main features for clustering. Before applying the algorithm I scaled the features using StandardScaler. To find the right number of clusters I used the elbow method by plotting inertia for different values of K. The elbow appeared at K equals 5 so I used that. After fitting K-Means I plotted the clusters on a 2D scatter plot with the centroids marked.

## Results

- Five distinct customer groups were identified
- One group has high income and high spending which are the most valuable customers
- Another group has low income but high spending indicating frequent buyers on a budget
- High income customers with low spending scores represent an untapped segment
- The clustering gives a clear basis for designing targeted marketing strategies
