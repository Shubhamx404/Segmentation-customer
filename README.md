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

# Data Exploration

![newplot](https://user-images.githubusercontent.com/25388109/86505481-152d9980-bdbd-11ea-9d45-5a8292671f31.png)

From the Map, You'll see that the dataset is largely dominated by orders made from this first five Countries

* `United Knigdom` with `19857` customers
* `Germany` with `603` customers
* `France` with `458` customers
* `EIRE` with `319` customers
* `Belgium` with `119` customers



#### keywords Word Occurence 

![word occurence 1](https://user-images.githubusercontent.com/25388109/86505722-4fe50100-bdc0-11ea-9a91-b4f971b594f3.png)
![word occurence 11](https://user-images.githubusercontent.com/25388109/86505724-52475b00-bdc0-11ea-8373-07fef750c573.png)
![keywords occurence 3](https://user-images.githubusercontent.com/25388109/86505803-11037b00-bdc1-11ea-84cc-7bae63eb13e1.png)



#### Product Content Word cloud

![word cloud](https://user-images.githubusercontent.com/25388109/86505858-8ec78680-bdc1-11ea-8fcc-5354a5767830.png)



#### PCA Customer category analysis

![PCA analysis 11](https://user-images.githubusercontent.com/25388109/86505918-18775400-bdc2-11ea-9508-40b33ddc3da9.png)


#### Customers morphology


![customer morphology 1](https://user-images.githubusercontent.com/25388109/86505974-a81d0280-bdc2-11ea-9eb7-cc42b2fe055a.png)
![customer morphology 11](https://user-images.githubusercontent.com/25388109/86505976-ac492000-bdc2-11ea-935b-c59341fecd37.png)



#### Classifiers and respective learning curves


![adaboost_learning_curve](https://user-images.githubusercontent.com/25388109/86506016-1feb2d00-bdc3-11ea-81bc-5ca083bf8916.png)
![decision_tree_learning curve](https://user-images.githubusercontent.com/25388109/86506017-211c5a00-bdc3-11ea-8813-0f0d7f3b2222.png)
![gradient_boosting_clf_learning_curve](https://user-images.githubusercontent.com/25388109/86506018-21b4f080-bdc3-11ea-916e-ee4270d2579b.png)
![knn_learning curve](https://user-images.githubusercontent.com/25388109/86506019-224d8700-bdc3-11ea-992c-e43120a2d454.png)
![lr_learning curve](https://user-images.githubusercontent.com/25388109/86506021-24afe100-bdc3-11ea-87ab-110886ca2f91.png)
![random_forest_learning_curve](https://user-images.githubusercontent.com/25388109/86506022-25487780-bdc3-11ea-88a8-5ba35d71c89f.png)


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
