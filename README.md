# Mall Customer Clustering Analysis

This project performs clustering analysis on the **Mall Customers dataset**, which contains customer information such as **Annual Income** and **Spending Score**.  
The goal is to group customers into meaningful segments using unsupervised learning techniques and compare different clustering models.

---

##  Objective
The analysis compares two clustering algorithms:
- **KMeans Clustering**
- **Agglomerative (Hierarchical) Clustering**

We evaluate their performance using internal validation metrics and visualize the clusters using PCA-reduced 2D plots.

---

##  Dataset
The dataset (`Mall_Customers.csv`) contains:
- `CustomerID`
- `Gender`
- `Age`
- `Annual Income (k$)`
- `Spending Score (1-100)`

For clustering, we focus mainly on:
- **Annual Income (k$)**
- **Spending Score (1-100)**

---

## Models Compared
1. **KMeans**  
   - Partitions customers into `k` clusters by minimizing within-cluster variance.  
   - Requires choosing number of clusters `k`.

2. **Agglomerative Clustering**  
   - A hierarchical bottom-up approach that merges clusters iteratively.  
   - Requires choosing number of clusters.

---

##  Evaluation Metrics
Since clustering is unsupervised, we use **internal evaluation metrics**:
- **Silhouette Score** → Higher is better (cohesive + well-separated clusters).
- **Calinski-Harabasz Index** → Higher means more distinct clusters.
- **Davies-Bouldin Index** → Lower indicates better clustering.

---

##  Visualizations
- PCA (2D reduction) scatter plots to visually compare cluster separation.  
- Side-by-side comparison of KMeans vs Agglomerative clustering.  

---

##  How to Run
1. Clone this repository and open the notebook:
   ```bash
   git clone https://github.com/HarmanBhangu1313/mall-customer-clustering
   cd mall-customer-clustering
   jupyter notebook Mall_Customer_Analysis.ipynb