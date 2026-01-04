# Customer_Behavior_Analysis# Customer Shopping Behavior – Data Cleaning & Analysis using Pandas

## 📌 Project Overview
This project focuses on cleaning, transforming, and preparing a customer shopping behavior dataset using **Python (Pandas) in Jupyter Notebook**. 

The objective is to demonstrate **end-to-end data handling** — from raw CSV ingestion to database integration — following best practices used in real-world analytics workflows.

---

## 📂 Dataset Description
The dataset contains **3,900 customer records** with attributes related to:
- Demographics (Age, Gender, Location)
- Purchase behavior (Item, Category, Amount, Frequency)
- Marketing variables (Discounts, Subscriptions)
- Customer feedback (Review Ratings)

---

## 🛠️ Tools & Technologies
- **Python**
- **Pandas**
- **Jupyter Notebook**

---

## 🔄 Steps Performed

### 1️⃣ Data Loading
- Imported dataset using `pandas.read_csv()`
- Verified successful ingestion by previewing records using `.head()`

---

### 2️⃣ Initial Data Exploration
- Examined dataset structure using `.info()`
- Generated descriptive statistics using `.describe(include='all')`
- Identified column types, ranges, and categorical distributions

---

### 3️⃣ Missing Value Handling
- Detected missing values in the **Review Rating** column
- Applied **category-wise median imputation** to preserve data distribution
- Ensured zero missing values post-imputation

**Why this matters:**  
Median imputation avoids skewing customer feedback metrics and maintains category-level consistency.

---

### 4️⃣ Column Standardization
- Converted column names to **snake_case**
- Renamed columns for clarity and SQL compatibility
  - Example: `Purchase Amount (USD)` → `purchase_amount`

---

### 5️⃣ Feature Engineering

#### 🔹 Age Group Creation
- Created a new column `age_group` using quartile-based segmentation:
  - Young Adult
  - Adult
  - Middle-aged
  - Senior

**Business value:**  
Enables customer segmentation and demographic analysis for targeted marketing.

---

#### 🔹 Purchase Frequency Normalization
- Converted categorical frequency values into numeric **days**
- Created `purchase_frequency_days` column

**Example:**
- Weekly → 7 days  
- Monthly → 30 days  
- Annually → 365 days

**Business value:**  
Allows quantitative modeling and customer lifetime value analysis.


---

### 7️⃣ Final Clean Dataset
- Final dataset contains:
  - Cleaned
  - Standardized
  - Feature-enhanced
  - Analysis-ready data

---

## 📊 Key Outcomes
- Cleaned and standardized **3,900 customer records**
- Engineered meaningful analytical features
- Eliminated redundant attributes
- Enabled seamless transition from analytics to databases

---

## 🚀 Future Scope
- Customer segmentation & clustering
- RFM analysis
- Predictive modeling
- Dashboarding using Power BI / Tableau

---

## 👩‍💻 Author
**Shivika Mahesh**  
Digital Marketing & Analytics Professional  
