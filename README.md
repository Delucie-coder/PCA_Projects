# Principal Component Analysis (PCA) from Scratch

This repository contains my individual implementation of **Principal Component Analysis (PCA)** using a dataset focused on African firms' capital structures. This project applies advanced linear algebra and multivariate probability concepts to perform dimensionality reduction while preserving maximum data variance.

## 📊 Project Overview

The objective is to transform a high-dimensional dataset (containing over 10 features) into a lower-dimensional space. This implementation is built from the ground up to demonstrate a deep understanding of the mathematical mechanics behind PCA.

### Key Implementation Details:

* **Data Handling**: Robust preprocessing of "Africanized" data, including handling of missing (NaN) values and encoding of non-numeric columns like "Company" and "Auditor".
* **Manual Standardization**: Implementation of the -score formula  to ensure all features contribute equally to the analysis.
* **Mathematical Core**: Calculation of the covariance matrix followed by eigendecomposition to extract eigenvalues and eigenvectors.
* **Dynamic Selection (Task 2)**: Algorithmic selection of the optimal number of principal components based on an explained variance threshold of 95%.
* **Visualization**: Comparative analysis showing the data structure in the original feature space versus the new principal component space.

---

## ⚙️ Installation Instructions

To run this notebook, ensure you have **Python 3.x** installed. You will need to install the following libraries to support the implementation and data processing:

### 1. Clone the Repository

```bash
git clone <your-github-repo-link>
cd <your-repo-name>

```

### 2. Install Dependencies

Install the required Python packages via pip:

```bash
pip install pandas numpy matplotlib

```

* **Pandas**: Used for dataset manipulation, handling missing values, and categorical encoding.
* **NumPy**: The primary library for matrix mathematics, manual standardization, and eigendecomposition.
* **Matplotlib**: Used for generating the "Before and After" 2D visualizations of the PCA results.



## 🚀 How to Use

1. **Data Placement**: Ensure the dataset `africa-capital-structure-firms.csv` is located in the root directory of the project.
2. **Open the Notebook**: Launch `Template_PCA_Formative_1.ipynb` in Google Colab or VS Code.
3. **Execution Steps**:
* **Standardization**: Run the cell to normalize the data manually using the -score formula.
* **Covariance & Eigenvectors**: Compute the directions of maximum variance.
* **Projection**: Project the original data onto the selected principal components.
* **Analysis**: Review the generated plots and the explained variance ratio to understand the dimensionality reduction effect.





## 📈 Results and Insight

The final output includes two primary visualizations:

1. **Before PCA**: Shows the distribution of the data based on the original standardized features.
2. **After PCA**: Shows the data rotated into the **PC1** and **PC2** axes. In this space, the axes are perfectly uncorrelated and ordered by the amount of variance they explain, with PC1 capturing the highest variance.
