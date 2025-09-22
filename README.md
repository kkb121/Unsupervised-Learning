# Unsupervised-Learning: Clustering Analysis of Population Datasets

This repository explores unsupervised clustering techniques on four synthetic datasets (pop1.csv, pop2.csv, pop3.csv, and pop4.csv).

The project implements and compares two clustering approaches:

	•	K-Means Clustering (with evaluation using Elbow and Silhouette methods)
	
	•	Gaussian Mixture Models (GMMs) (with evaluation using the Bayesian Information Criterion, BIC)

It also provides a visual and analytical comparison between the results from K-Means and GMMs.


The script will:
	1.	Load the four population datasets
	2.	Perform K-Means clustering with 2–10 clusters
	3.	Evaluate clustering performance using:
		•	Elbow Method
		
		•	Silhouette Analysis
	4.	Fit Gaussian Mixture Models (GMM)
	5.	Evaluate with BIC scores
	6.	Compare K-Means and GMM results visually


Implemented Methods

1. K-Means Clustering
	•	Applied to all four populations
	•	Cluster visualisation with centroids
	•	Evaluation methods:
	•	Elbow method (based on inertia/SSE)
	•	Silhouette coefficient (cluster separation/density)

2. Gaussian Mixture Models (GMM)
	•	Fitted to all populations
	•	Evaluated with the Bayesian Information Criterion (BIC)
	•	Helps avoid overfitting compared to raw log-likelihood

3. Comparison Framework
	•	Side-by-side visual comparison of:
	•	Elbow method (inertia)
	•	Silhouette scores
	•	GMM BIC scores



Key Findings
	•	Pop1: Best clustered with 2 clusters (very high silhouette score ~0.94)
	•	Pop2: Elbow and Silhouette suggest 2–3 clusters
	•	Pop3: Optimal around 5 clusters (Silhouette ~0.49)
	•	Pop4: Clear separation at 3 clusters (Silhouette ~0.87)
	•	GMM vs K-Means:
	•	K-Means works well for spherical, evenly sized clusters
	•	GMM provides flexibility for overlapping, non-spherical clusters and can capture distributions better in some datasets
