## Customer Segmentation using RFM Analysis and Clustering

This project applies **RFM (Recency, Frequency, Monetary) Analysis** and **K-Means Clustering** to segment customers based on their purchasing behavior. This segmentation helps businesses identify different customer groups to personalize marketing strategies, improve retention, and increase revenue.

---

### 📊 Dataset
- **Source:** Online Retail dataset  
- **Features Used:**
  - `CustomerID`
  - `InvoiceDate`
  - `InvoiceNo`
  - `Quantity`
  - `UnitPrice`

---

###  Tools & Technologies
- **Languages & Libraries:** Python, Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
- **Environment:** Jupyter Notebook

---

###  Methodology
#### 1. Data Cleaning & Preprocessing
- Removed missing values and canceled transactions.
- Derived `TotalPrice = Quantity × UnitPrice`.

#### 2. RFM Metric Calculation
- **Recency:** Days since last purchase
- **Frequency:** Number of transactions
- **Monetary:** Total spent

#### 3. RFM Scoring & Segmentation
- Each RFM metric was scored on a scale of 1–5.
- Customers were grouped using RFM scores and clustered using K-Means.

#### 4. Clustering
- Used the **Elbow Method** to determine optimal clusters.
- Applied **K-Means Clustering** on normalized RFM data.
- Visualized clusters using scatter plots and box plots.
-  ![RFM Cluster Plot](rfm_clusters.png)

---
### 📌 Key Insights
- **Champions:** High-value, frequent buyers with recent purchases.
- **At-Risk Customers:** Previously valuable but inactive lately.
- **Loyal Customers:** Consistent and frequent buyers.
- **Potential Loyalists:** Recent buyers with potential to become loyal.

---

### Business Impact
- Helps in **personalized marketing**, **loyalty programs**, and **customer retention**.
- Enables **data-driven decision-making** for targeted campaigns.
