<!-- README: Unsupervised-Learning: Clustering Analysis of Population Datasets -->
<h1>Unsupervised-Learning: Clustering Analysis of Population Datasets</h1>

<p>
  This repository explores <strong>unsupervised clustering techniques</strong> on four synthetic datasets 
  (<code>pop1.csv</code>, <code>pop2.csv</code>, <code>pop3.csv</code>, and <code>pop4.csv</code>).
</p>

<p>The project implements and compares two clustering approaches:</p>
<ul>
  <li><strong>K-Means Clustering</strong> (with evaluation using Elbow and Silhouette methods)</li>
  <li><strong>Gaussian Mixture Models (GMMs)</strong> (with evaluation using the Bayesian Information Criterion, BIC)</li>
</ul>

<p>It also provides a visual and analytical comparison between the results from K-Means and GMMs.</p>

<hr>

<h2 id="workflow">Workflow</h2>
<ol>
  <li>Load the four population datasets</li>
  <li>Perform K-Means clustering with 2–10 clusters</li>
  <li>
    Evaluate clustering performance using:
    <ul>
      <li>Elbow Method</li>
      <li>Silhouette Analysis</li>
    </ul>
  </li>
  <li>Fit Gaussian Mixture Models (GMM)</li>
  <li>Evaluate with BIC scores</li>
  <li>Compare K-Means and GMM results visually</li>
</ol>

<hr>

<h2 id="implemented-methods">Implemented Methods</h2>

<h3>1. K-Means Clustering</h3>
<ul>
  <li>Applied to all four populations</li>
  <li>Cluster visualisation with centroids</li>
  <li>
    <strong>Evaluation methods:</strong>
    <ul>
      <li>Elbow method (based on inertia/SSE)</li>
      <li>Silhouette coefficient (cluster separation/density)</li>
    </ul>
  </li>
</ul>

<h3>2. Gaussian Mixture Models (GMM)</h3>
<ul>
  <li>Fitted to all populations</li>
  <li>Evaluated with the <strong>Bayesian Information Criterion (BIC)</strong></li>
  <li>Helps avoid overfitting compared to raw log-likelihood</li>
</ul>

<h3>3. Comparison Framework</h3>
<ul>
  <li>Side-by-side visual comparison of:
    <ul>
      <li>Elbow method (inertia)</li>
      <li>Silhouette scores</li>
      <li>GMM BIC scores</li>
    </ul>
  </li>
</ul>

<hr>

<h2 id="key-findings">Key Findings</h2>
<ul>
  <li><strong>Pop1:</strong> Best clustered with 2 clusters (very high silhouette score ~0.94)</li>
  <li><strong>Pop2:</strong> Elbow and Silhouette suggest 2–3 clusters</li>
  <li><strong>Pop3:</strong> Optimal around 5 clusters (Silhouette ~0.49)</li>
  <li><strong>Pop4:</strong> Clear separation at 3 clusters (Silhouette ~0.87)</li>
  <li><strong>K-Means vs GMM:</strong>
    <ul>
      <li>K-Means works well for spherical, evenly sized clusters</li>
      <li>GMM provides flexibility for overlapping, non-spherical clusters and can capture distributions better in some datasets</li>
    </ul>
  </li>
</ul>
