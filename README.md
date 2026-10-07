# Fraud Detection & Graph Analytics

A collection of fraud detection and risk analytics approaches developed as part of coursework at **IIT Hyderabad**, exploring transaction-network analysis, graph representation learning, trust propagation, spectral methods, and cost-sensitive machine learning.

## Overview

This project explores multiple approaches for analysing potentially fraudulent or anomalous behaviour in dealer transaction networks.

The work covers:

* **Graph representation learning** for identifying potential circular-trade relationships
* **Trust propagation** for ranking dealer reliability in transaction networks
* **Spectral graph methods** for identifying potential outlier dealers
* **Cost-sensitive classification** for fraud screening under asymmetric false-negative costs

## Project Components

### 1. Circular Trade Detection

**Techniques:** NetworkX · Node2Vec · K-Means · Graph Analytics

Modelled seller–buyer relationships as a directed multigraph and generated node embeddings using Node2Vec. K-Means clustering and transaction-value criteria were then used to identify potential circular-trade relationships.

**Dataset:** 130,535 transaction records across 799 dealers  
**Result:** Flagged 16 potential dealer pairs for further investigation.

**Repository:** [View Circular Trade Detection →](https://github.com/Sindhuja-5/circular-trade-detection)

---

### 2. TrustRank using Pregel

**Techniques:** Pregel · TrustRank · Graph Processing · Message Passing

Implemented TrustRank on a dealer transaction network, using known untrustworthy dealers to initialize trust information and iteratively propagating scores across transaction relationships to rank dealer reliability.

**Repository:** [View TrustRank using Pregel →](https://github.com/Sindhuja-5/Trust-Rank-Pregel)

---

### 3. Dealer Outlier Detection

**Techniques:** Gaussian-Kernel Similarity · Graph Laplacian · Spectral Methods · K-Means

Constructed a similarity graph from dealer correlation and ratio features, computed the graph Laplacian eigenspace, and applied K-Means clustering to identify potentially anomalous dealers.

**Result:** Flagged 398 potential outlier dealers.

**Repository:** [View Dealer Outlier Detection →](https://github.com/Sindhuja-5/Dealer-Outlier-Detection)

---

### 4. Cost-Sensitive Binary Classification

**Techniques:** Keras · Scikit-learn · Binary Classification · Cost-Sensitive Learning

Built a Keras-based binary classification model incorporating observation-specific false-negative costs into threshold-based classification for cost-aware fraud screening.

**Dataset:** 147,636 observations and 11 predictive variables

**Repository:** [View Cost-Sensitive Classification →](https://github.com/Sindhuja-5/Cost-Sensitive-Logistic-Regression)

---

## Technical Skills

**Programming:** Python

**Data & Machine Learning:** Pandas · NumPy · Scikit-learn · Keras

**Graph & Network Analysis:** NetworkX · Node2Vec · Pregel · Graph Laplacian · Spectral Methods

**Machine Learning Methods:** K-Means Clustering · Binary Classification · Cost-Sensitive Learning · Graph Representation Learning

## Academic Context

Developed as part of **Fraud Analytics  using Predictive and Social Network Techniques coursework at IIT Hyderabad**.

**Degree:** B.Tech. Mathematics & Computing  
**Institution:** Indian Institute of Technology Hyderabad
