# Customer Segmentation Analysis using K-Means Clustering and Power BI

## Overview

Customer Segmentation is one of the most important applications of unsupervised learning. Using clustering techniques, companies can identify several segments of customers, allowing them to target the potential user base more efficiently. In this project, we use **K-Means Clustering** to discover patterns in customer behavior. A Power BI dashboard complements the analysis by visually highlighting trends and demographics.

---

## What is Customer Segmentation?

Customer Segmentation is the process of dividing a customer base into distinct groups of individuals that share similarities in various aspects like age, gender, income, and spending habits.

Organizations use segmentation to:

* Personalize marketing strategies
* Understand customer needs more precisely
* Minimize risk and improve ROI

Segmentation depends on demographic, geographic, and behavioral data to identify high-value clusters for strategic planning.

---

## What is the K-Means Algorithm?

K-Means is an unsupervised learning algorithm that groups unlabeled data into "k" clusters:

1. Choose the number of clusters (k)
2. Randomly select initial centroids
3. Assign each data point to the nearest centroid using Euclidean distance
4. Recalculate centroids and repeat until convergence

The goal is to minimize the **within-cluster sum of squares (WCSS)**, leading to compact, well-separated clusters.

---

## Dataset

* **Source:** [Kaggle – Mall Customer Segmentation](https://www.kaggle.com/nelakurthisudheer/mall-customer-segmentation)
* **Attributes:**

  * `CustomerID`: Unique customer ID
  * `Gender`: Male or Female
  * `Age`: Age of the customer
  * `Annual Income (k$)`: Yearly income in \$1000s
  * `Spending Score (1-100)`: Score assigned based on behavior and spending patterns

---

## Project Steps

### 1. Data Preprocessing

* Imported the CSV file
* Cleaned and explored the data
* Converted categorical features if needed

### 2. Exploratory Data Analysis (EDA)

* Distribution plots of `Age`, `Income`, `Spending Score`
* Gender comparison using bar and pie charts
* Box plots and density plots to analyze variability

### 3. Clustering with K-Means

* Selected features: `Age`, `Income`, `Spending Score`
* Determined optimal clusters using:

  * **Elbow Method**
  * **Silhouette Score**
  * **Gap Statistic**
* Final model used optimal cluster value (e.g., k=5)
* Visualized clusters using PCA (Principal Component Analysis)

### 4. Power BI Dashboard

The dashboard summarizes the analysis with interactive visuals:

* **KPI Cards**: Total customers, Avg Age, Avg Income, Total Spending Score
* **Pie Chart**: Gender Distribution
* **Bar Charts**: Avg Spending by Gender, Spending vs Income Trends
* **Scatterplots**: Income vs Spending across Age Groups

---

## Key Insights

* Male and Female customers have nearly equal distribution
* Certain age groups (e.g., 30–40) show higher spending behavior
* High-income groups don't always correlate with high spending scores

---

## Folder Structure

```
Customer-Segmentation-Analysis/
├── Dataset/
│   └── Mall_Customers.csv
├── JupyterNotebook/
│   └── Customer_Segmentation_Analysis.ipynb
├── PowerBI_Report/
│   └── Customer Segmentation Dashboard.pbix
├── Dashboard_Screenshot/
│   └── Dashboard.png
└── README.md
```

---

## Tools & Technologies Used

* **Python**: Data analysis and K-means clustering (with Pandas, Matplotlib, Seaborn, Scikit-learn)
* **Power BI**: Dashboard and reporting
* **Jupyter Notebook**: Data processing pipeline

---

## Conclusion

This project successfully demonstrates how unsupervised learning can segment customers effectively. By identifying different behavioral clusters, businesses can better understand their customers and craft more targeted marketing strategies. The combination of clustering and dashboarding makes this project highly insightful and practical.

---

## Author

* **Project by:** \Lingeshwaran G 
* **LinkedIn:** \https://www.linkedin.com/in/lingeshdev/
* **GitHub:** \https://github.com/LingeshDev
