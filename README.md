# **PayTrack: AI-Powered Payment Forecasting**  

## **📌 Overview**  
**PayTrack** is an **AI-powered system** designed to **predict invoice payment dates** using **machine learning (ML)**. By analyzing historical payment patterns, PayTrack helps businesses **forecast cash flow, reduce overdue payments, and optimize financial planning**.  

---

## **1️⃣ Project Workflow**  

### **🔹 Step 1: Data Preprocessing**  
- Handle **missing values** in payment records.  
- Convert **dates to datetime format** (invoice date, due date, payment date).  
- Detect and remove **outliers** in payment delays.  

### **🔹 Step 2: Exploratory Data Analysis (EDA)**  
- Analyze **customer payment behaviors** (early, on-time, late payments).  
- Visualize **payment delay distributions** using histograms and box plots.  
- Identify **seasonal trends** affecting payment timelines.  

### **🔹 Step 3: Feature Engineering & Extraction**  
✅ **Date-based Features:**  
- **Days until due:** `(due_date - invoice_date).days`  
- **Days delayed:** `(payment_date - due_date).days`  
- Extract **Month, Year, Quarter** from invoice dates.  

✅ **Customer-based Features:**  
- **Average past payment delay**  
- **Late payment frequency**  
- **Customer reliability score**  

✅ **Invoice-based Features:**  
- **Invoice amount**  
- **Invoice type (recurring vs one-time payments)**  

### **🔹 Step 4: Machine Learning Model - XGBoost Regression**  
- **Supervised Learning Approach:** Trains on past invoices to predict future payment dates.  
- **Algorithm Used:** **XGBoost Regression** for high accuracy and efficiency.  
- **Model Training:**  
  - **Input Features:** `days_until_due, invoice_amount, month, year`  
  - **Target Variable:** `days_delayed`  

### **🔹 Step 5: Model Evaluation**  
📌 **Metrics Used:**  
- **Mean Absolute Error (MAE)** – Measures average days of prediction error.  
- **Root Mean Squared Error (RMSE)** – Penalizes large errors more.  

---

## **2️⃣ Technologies Used**  
🔹 **Python** – Core implementation  
🔹 **Pandas & NumPy** – Data processing & feature engineering  
🔹 **Seaborn & Matplotlib** – Data visualization  
🔹 **XGBoost** – Machine learning model for regression  

---  

---

## ** Expected Outcome**  
✅ **Accurate prediction of invoice payment dates**  
✅ **Better financial planning for businesses**  
✅ **Identification of high-risk customers with late payments**  

---
