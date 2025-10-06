# 🛍️ Mall Customers Clustering & Segmentation

## 📌 Project Overview
This project performs **Customer Segmentation** using clustering algorithms to identify patterns in mall customers' demographics, income, and spending behavior.  
The dataset is sourced from **Kaggle** (`Mall_Customers.csv`), containing customer demographics and spending scores.  
The goal is to provide actionable insights for **targeted marketing strategies**.

---

## 🎯 Objectives
- Segment customers into meaningful groups.
- Understand the relationship between **Age, Gender, Income, and Spending Score**.
- Compare the effectiveness of **KMeans**, **DBSCAN**, and **Agglomerative Clustering**.
- Provide business recommendations based on findings.

---

## 📂 Dataset Information
**Source:** [Kaggle - Customer Segmentation](https://www.kaggle.com/datasets/joebeachcapital/customer-segmentation)  
**File:** `Mall_Customers.csv`  
**Columns:**
- `CustomerID` - Unique customer identifier
- `Gender` - Male / Female
- `Age` - Age of customer
- `Annual Income (k$)` - Yearly income in thousands
- `Spending Score (1-100)` - Assigned score by mall based on spending behavior

---

## 🛠️ Tech Stack
- **Language:** Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)  
- **Clustering Algorithms:** KMeans, DBSCAN, Agglomerative (Hierarchical) Clustering  
- **Visualization:** Matplotlib, Seaborn, 3D Scatter Plots  
- **Data Source:** KaggleHub API  

---

## 📊 Methodology
1. **Data Loading & Cleaning**
   - Downloaded dataset via KaggleHub
   - Set `CustomerID` as index
   - Encoded `Gender` (Male → 0, Female → 1)

2. **Exploratory Data Analysis (EDA)**
   - Correlation heatmaps
   - Scatter plots for visualizing clusters

3. **KMeans Clustering**
   - Used **Elbow Method** to determine optimal clusters
   - Segmented customers into **4 clusters**
   - Evaluated with **Silhouette Score**

4. **Agglomerative Clustering**
   - Created dendrogram to analyze linkage distances
   - Segmented into 4 hierarchical clusters
   - Compared results with KMeans

5. **3D Visualization**
   - Plotted Age, Annual Income, and Spending Score to visualize cluster separation

---

## 📈 Results & Insights

### 🔍 Key Findings
- **Cluster 0:** Low income, low spending → price-sensitive customers.
- **Cluster 1:** High income, high spending → premium customers, ideal for upselling.
- **Cluster 2:** Average income, average spending → potential for loyalty programs.
- **Cluster 3:** High income, low spending → untapped potential, needs re-engagement.

- **Silhouette Score (KMeans):** ~0.55 → Good separation between clusters.
- **Silhouette Score (Agglomerative):** Slightly lower, indicating KMeans was more effective.

---

## 💡 Recommendations
- **Premium customers (High income & high spending)** → Introduce exclusive VIP programs and luxury offerings.
- **Price-sensitive customers** → Focus on discounts, bundles, and promotions.
- **Average spenders** → Loyalty points and referral bonuses.
- **High income but low spending** → Personalized marketing, event invites, and targeted product recommendations.

---
