# 🛍️ E-Commerce Customer Segmentation

This project analyzes customer purchasing behavior on an e-commerce platform and segments customers into meaningful groups using clustering techniques.  
The goal is to understand customer patterns to improve marketing strategies, personalize offers, and enhance user retention.

---

## 📊 Project Overview

The dataset contains transactional information about customers’ purchases over a period of one year.  
Each record represents a purchase made by a customer, including details such as product, date, and price.

Using **K-Means Clustering**, **RFM Analysis**, and **Visualization techniques**, we identify unique customer groups and interpret their shopping behavior.

---

## 🧠 Objectives

- Segment customers based on purchase behavior  
- Identify high-value and at-risk customers  
- Provide actionable insights for targeted marketing  
- Visualize data trends and cluster distributions

---

## 📁 Dataset

| Column | Description |
|--------|--------------|
| `CustomerID` | Unique identifier for each customer |
| `InvoiceNo` | Transaction ID |
| `InvoiceDate` | Date of purchase |
| `Quantity` | Number of products purchased |
| `UnitPrice` | Price per product |
| `Country` | Customer’s country |

📦 **Total customers:** ~4000  
🛒 **Period:** 1 year of transactions  

---

## ⚙️ Methodology

1. **Data Cleaning**
   - Handle missing and duplicate values  
   - Remove invalid transactions (e.g., negative quantities)

2. **Feature Engineering**
   - Compute *Recency, Frequency, and Monetary (RFM)* values for each customer

3. **Normalization**
   - Scale RFM scores using MinMaxScaler or StandardScaler

4. **Modeling**
   - Apply **K-Means Clustering** to group customers  
   - Use **Elbow Method** and **Silhouette Score** to determine the optimal number of clusters

5. **Visualization**
   - Visualize clusters and their characteristics using **Matplotlib** and **Seaborn**

---

## 📈 Results & Insights

- **Cluster 0** – Loyal, high-value customers  
- **Cluster 1** – Occasional shoppers with moderate spending  
- **Cluster 2** – New or low-spend customers  

These insights can guide marketing teams to:
- Offer loyalty rewards to Cluster 0  
- Send re-engagement campaigns to Cluster 2  
- Promote upselling to Cluster 1  

---

## 📊 Visualizations

Below are key visual insights from the notebook:

![RFM Distribution](assets/rfm_distribution.png)
![Cluster Visualization](assets/customer_clusters.png)
![Elbow Method](assets/elbow_method.png)
![Silhouette Score](assets/silhouette_score.png)
![Spending Patterns](assets/spending_patterns.png)

> 💡 You can replace these with your actual output graphs from the notebook.

---

## 🧩 Technologies Used

- **Python**  
- **Pandas**, **NumPy**  
- **Matplotlib**, **Seaborn**, **Plotly**  
- **Scikit-learn**

---

## 🚀 How to Run

```bash
# 1️⃣ Clone this repository
git clone https://github.com/<your-username>/customer-segmentation.git

# 2️⃣ Navigate to the folder
cd customer-segmentation

# 3️⃣ Install dependencies
pip install -r requirements.txt

# 4️⃣ Run the notebook
jupyter notebook CUSTOMER_SEGMENT.ipynb
