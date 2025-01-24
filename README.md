# 📊 Project: Marketing Campaign Clustering and Analysis

A comprehensive data analysis and clustering project exploring customer segmentation for marketing campaigns. This project covers data preparation, feature engineering, dimensionality reduction, clustering, and visualization.

---

## 📁 Dataset Preparation

- **Dataset**: `marketing_campaign.csv`  
  - Source: Internal customer database.  
  - Format: Tab-separated values (`.csv`).

- **Steps Taken**:
  - Handled missing values by:
    - Dropping rows with null values (low proportion of missing data).
  - Converted date fields (`Dt_Customer`) to datetime format for feature engineering.
  - Encoded categorical variables for further analysis.

---

## 🔍 Feature Engineering

- Created new features for better insights and clustering:
  - **Customer_For**: Number of days a customer has been with the company, calculated relative to the most recent customer.
  - **Age**: Derived from the `Year_Birth` column.
  - **Amount_Spent**: Total spending on various product categories (Wines, Fruits, Meat, etc.).
  - **Living_With**: Simplified marital status into broader categories (e.g., Partner, Alone).
  - **Children**: Combined `Kidhome` and `Teenhome` columns to indicate total children.
  - **Family_Size**: Defined based on living status and children.
  - **IS_Parent**: Binary feature indicating parenthood.
  - Simplified **Education** levels (e.g., Graduated, PostGraduate, UnderGraduate).

- Dropped redundant or irrelevant features:
  - `Marital_Status`, `Dt_Customer`, `Z_CostContact`, `Z_Revenue`, etc.

---

## 🛠️ Dimensionality Reduction

- Applied **Principal Component Analysis (PCA)**:
  - Reduced dimensions to 3 for better visualization and clustering.
  - Retained maximum variance in the data while reducing complexity.

---

## 🤖 Clustering

- **Method**: Agglomerative Clustering (Hierarchical Clustering).
- **Steps Taken**:
  - Determined the optimal number of clusters using the elbow method.
  - Clustered data into 4 groups based on reduced dimensions.
  - Visualized clusters in both 3D and 2D plots.

---

## 📊 Visualization

- Plotted relationships between features to analyze:
  - Spending patterns (`Amount_Spent` vs. `Income`).
  - Product preferences (e.g., spending on Wines).
  - Cluster distributions and profiles.
- Used a custom color palette to enhance clarity and presentation.

---

## 🏆 Results and Insights

- Identified distinct customer groups based on spending behavior and demographics.
- Gained insights into product preferences and income distribution within clusters.
- Highlighted potential target groups for personalized marketing strategies.

---

## 📄 Documentation

This project includes:
- A well-documented Python script showcasing the complete workflow.
- Clear visualizations to aid in understanding customer segmentation.

---

## 🙌 Acknowledgments

- Libraries used:
  - **Pandas**, **NumPy** for data manipulation.
  - **Seaborn**, **Matplotlib** for visualization.
  - **Scikit-learn** for PCA and clustering.
- Data preprocessing and clustering techniques inspired by industry practices.

---

## 📬 Contact

For any questions or suggestions, feel free to reach out:

- **Name**: G. Kamesh
- **Email**: [kamesh743243@gmail.com](mailto:kamesh743243@gmail.com)  
