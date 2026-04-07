# Fashion-MNIST Classification using Complete Kernel Fisher Discriminant (CKFD)

This project implements a sophisticated classification pipeline for the **Fashion-MNIST** dataset using the **Complete Kernel Fisher Discriminant (CKFD)** algorithm. The approach combines PCA for initial dimensionality reduction with Kernel-based LDA to extract features from both regular and irregular subspaces.

## Features
* **Automated Preprocessing:** Data cleaning (NaN/Inf handling), Standard Scaling, and PCA (retaining 90% of variance).
* **CKFD Implementation:** Complete Kernel Fisher Discriminant analysis with support for:
    * **Linear** Kernel
    * **Polynomial** Kernel (various degrees)
    * **RBF** (Gaussian) Kernel
* **Dual Subspace Learning:** Feature extraction from both **Regular** and **Irregular** subspaces to maximize discriminative power.
* **Classification Models:** Performance comparison between:
    * **1-Nearest Neighbor (1-NN)**
    * **Nearest Centroid Classifier (NCC)**
* **Visualizations:** * Cumulative Explained Variance plots.
    * Confusion Matrices for performance analysis.
    * Sample displays of Correct vs. Incorrect classifications with labels.

## Results & Evaluation
The model automatically iterates through various kernel configurations to identify the optimal parameters. 
- **Model Selection:** The winning kernel is selected based on Validation Accuracy.
- **Metrics:** Comprehensive evaluation using Precision, Recall, and F1-Score via Scikit-Learn's classification report.
