# Principal Component Analysis (PCA) from Scratch: African Firms Capital Structure

This repository contains an individual implementation of **Principal Component Analysis (PCA)** using a dataset focused on the capital structures of African firms. The project applies multivariate statistics and linear algebra to reduce the dimensionality of financial data while preserving maximum variance.

## 📊 Project Overview

The objective is to transform a high-dimensional financial dataset (containing 37 features) into a lower-dimensional space. This implementation is built manually to demonstrate a deep understanding of the mathematical mechanics behind dimensionality reduction.

### Key Implementation Details:

* **Robust Preprocessing**: Automated identification and encoding of categorical features (e.g., "Company", "Auditor") and mean imputation for missing (NaN) values.
* **Manual Standardization**: Implementation of the -score formula  using NumPy to ensure all financial metrics contribute equally.
* **Mathematical Core**: Calculation of the covariance matrix followed by eigendecomposition to extract principal directions of variance.
* **Dynamic Selection (Task 2)**: Algorithmic selection of the optimal number of components required to capture 95% of the total variance.
* **Optimization (Task 3)**: Use of vectorized matrix operations to ensure the algorithm handles large-scale datasets effectively.


## 📈 Visual Analysis

### 1. Eigenvalue Spectrum (Scree Plot)

The Scree Plot visualizes how much information (variance) is captured by each principal component. This allows us to justify the reduction of 37 features down to the primary components that explain 95% of the data's behavior.

### 2. Dimensionality Reduction (Before vs. After)

The results include a side-by-side comparison of the data in its original feature space versus the new **PC1** and **PC2** axes. In the PCA space, the axes are perfectly uncorrelated and ordered by the amount of variance they explain.

### 3. Performance Scaling

To satisfy Task 3, the project includes a benchmark demonstrating that the execution time scales linearly with the number of samples, proving the efficiency of the optimized manual implementation.


## ⚙️ Setup and Usage

### 1. Installation

Ensure you have Python 3.x and the following libraries installed:

```bash
pip install pandas numpy matplotlib

```

### 2. Running the Analysis

1. Place `africa-capital-structure-firms.csv` in the root directory.
2. Open `PCA_Formative_2[Delucie_Rurangwa].ipynb` in VS Code or Google Colab.
3. Run all cells to perform the data cleaning, PCA transformation, and benchmarking.
