# Wholesale Customers Data Analysis & Segmentation Pipeline

This repository contains an end-to-end unsupervised learning pipeline designed to perform customer segmentation using the Wholesale Customers dataset. The project demonstrates advanced exploratory data analysis (EDA), data transformations for highly skewed data, dimensionality reduction, and density-based vs. centroid-based clustering evaluations.

## 🛠️ Tech Stack & Core Libraries
* **Language:** Python 3.13
* **Libraries:** Pandas, NumPy, Scikit-Learn, UMAP-learn, Matplotlib, Seaborn
* **Environment:** Jupyter Notebook

## ⚙️ Engineering Workflow & Implementation Details

The notebook processes multi-dimensional wholesale purchase data through a strict analytical pipeline:

1. **Data Integrity & Structural Analysis:**
   * Audited dataset dimensions and explicitly mapped out variable types (Continuous vs. Nominal Categorical).
   * Conducted missing value verifications and initial statistical summary analysis.
2. **Advanced Data Transformation:**
   * **Outlier Analysis & Impact Evaluation:** Evaluated how extreme wholesale purchase values distort traditional clustering.
   * **Log Transformation:** Applied statistical log transformations to mitigate high right-skewness across feature distributions before scaling.
   * **Feature Scaling:** Implemented and compared `StandardScaler` and `RobustScaler` to normalize dimensions appropriately for distance-based algorithms.
3. **Dimensionality Reduction:**
   * Leveraged **UMAP (Uniform Manifold Approximation and Projection)** to project high-dimensional purchase variables into a lower-dimensional space while preserving local and global geometric structures.
4. **Clustering & Segmentation Orchestration:**
   * **K-Means Clustering:** Implemented centroid-based grouping to segment clients based on spending patterns.
   * **DBSCAN Clustering:** Deployed density-based clustering to handle complex shapes and natively isolate noise/outliers (interpreted unclassified noise points systematically).
   * **Cluster Interpretation:** Provided comprehensive profiles of customer groups to translate mathematical clusters into actionable business archetypes.

## 📂 Repository Contents
* `customer_segmentation.ipynb` -> Core Jupyter Notebook containing data pipeline executions and markdown reports.
* `Wholesale customers data.xls` -> Local source dataset containing client annual spending data across product categories.
* `README.md` -> Technical overview of the project architecture.

## 🚀 Getting Started
1. Clone the repository:
   ```bash
   git clone [https://github.com/pd8r/Wholesale-Customer-Segmentation.git](https://github.com/pd8r/Wholesale-Customer-Segmentation.git)

2. Install the necessary dependencies (including UMAP and excel engines):
   ```bash
   pip install pandas numpy scikit-learn umap-learn matplotlib seaborn openpyxl jupyter

3. Launch the server:
   ```bash
   jupyter notebook
  

