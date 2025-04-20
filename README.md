# 🛍️ Customer Segmentation using K-Means and DBSCAN

This project focuses on segmenting customers from the **Online Retail Dataset** using clustering techniques like **K-Means** and **DBSCAN**. It leverages key features like **total spending** and **purchase interval** to group customers based on behavioral patterns.

---

## 📂 Dataset

- Source: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/machine-learning-databases/00352/Online%20Retail.xlsx)
- Contains transactions from a UK-based and registered non-store online retail.

---

## 🧰 Libraries Used

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib`

---

## 📊 Features Engineered

- **Total_Bill**: Quantity × UnitPrice
- **Total_Bill_Size**: Total purchase value per customer
- **Purchase_Interval_Days**: Days between first and last purchase
- **Most_Common_Location**: Country where the customer most frequently purchased from
- **Top_Item**: Most frequently bought item by the customer

---

## 🚀 K-Means Clustering Approach

1. Standardized the `Total_Bill_Size`.
2. Applied **K-Means** with `n_clusters=3`.
3. Clustered customers based on their spending patterns.
4. Summarized each cluster:
   - Number of customers
   - Average spend
   - Top locations
   - Top items

### 📌 Insights

- Identified high spenders and frequent buyers.
- Clustered similar spending behaviors together.
- Helped understand which items and locations dominate per segment.

---

## 🔍 DBSCAN Clustering Approach

1. Used `Total_Bill_Size` and `Purchase_Interval_Days`.
2. Applied **DBSCAN** with `eps=0.5`, `min_samples=5`.
3. Detected **3 clusters** and **noise points**.
4. Plotted the results and summarized each cluster.

### 📌 Insights

- Robust against noise (outliers).
- Detected a few high-value customer clusters.
- Revealed customer activity duration patterns.

---

## 📈 Visualization

- Scatter plot shows clusters using DBSCAN with color-coded labels.
- Each point represents a customer scaled by spending and interval.

---

## 📁 File Structure

```bash
📦 customer-segmentation
├── kmeans_customer_segmentation.py
├── dbscan_customer_segmentation.py
├── README.md
