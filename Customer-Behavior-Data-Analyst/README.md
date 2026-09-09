# 📊 Customer Behavior Data Analyst

A complete end-to-end **Data Analytics project** that analyzes customer purchasing behavior using **Python, SQL, and Power BI**.
This project simulates a real-world business environment and demonstrates how raw data can be transformed into actionable business insights — from a stated business problem, through cleaning and EDA, to SQL analysis, a Power BI dashboard, and a stakeholder-ready presentation.

<img width="4872" height="2656" alt="CBA" src="https://github.com/user-attachments/assets/192f1038-25fb-45d4-8b0f-f2d867624e1d" />

---

## 🎯 Project Objective
The goal of this project is to replicate a real data analyst workflow, starting from a defined business problem rather than an open-ended dataset:

- Define the business problem  
- Clean and prepare raw customer data  
- Perform exploratory data analysis (EDA)  
- Write business-driven SQL queries  
- Build an interactive Power BI dashboard  
- Summarize insights and recommendations for stakeholders  

---

## 🧱 Project Workflow

### 1️⃣ Data Cleaning & EDA (Python)
- Missing-value imputation (review ratings filled by category median)
- Feature engineering: `age_group` (quartile-based) and `purchase_frequency_days`
- Column standardization (snake_case) and redundant-column removal, verified before dropping
- Exploratory analysis: purchase amount distribution, revenue by gender, top items, spend by age group, subscriber vs. non-subscriber spend, review rating distribution, and a correlation heatmap

**Libraries used:** Pandas, NumPy, Matplotlib, Seaborn

### 2️⃣ SQL Analysis
- Load the cleaned dataset into a database
- 10 business-driven SQL queries covering revenue by gender, discount behavior, top-rated and top-selling products, shipping comparisons, subscription impact, customer segmentation (New/Returning/Loyal via a CTE), and revenue by age group
- Uses CTEs, window functions (`ROW_NUMBER() OVER (PARTITION BY ...)`), and conditional aggregation

**Database:** PostgreSQL / MySQL / SQL Server (connection examples for all three are in the notebook)

### 3️⃣ Power BI Dashboard
- Interactive dashboard with KPI cards, customer segmentation, revenue trends, and category performance, built on the same business questions answered in SQL

---

## 🛠️ Tech Stack
Python · SQL · Power BI · Jupyter Notebook · Git & GitHub

---

## 📂 Repository Structure
```
Customer-Behavior-Data-Analyst/
│
├── notebooks/
│   └── Customer_Shopping_Behavior_Analysis.ipynb   # cleaning, feature engineering, EDA
│
├── sql/
│   └── customer_behavior_sql_queries.sql           # 10 business-driven queries
│
├── dashboard/
│   └── customer_behavior_dashboard.pbix            # Power BI dashboard
│
├── data/
│   └── customer_shopping_behavior.csv              # raw dataset (3,900 records)
│
├── docs/
│   ├── Business Problem Document.pdf                # problem framing / stakeholder ask
│   ├── Customer Shopping Behavior Analysis.pdf       # written analysis report
│   └── Customer-Shopping-Behavior-Analysis.pptx      # stakeholder presentation deck
│
├── requirements.txt
├── LICENSE
└── README.md
```

---

## 🚀 How to Run the Project

### Step 1: Clone the repository
```bash
git clone https://github.com/Anurag-M1/Customer-Behavior-Data-Analyst.git
cd Customer-Behavior-Data-Analyst
```

### Step 2: Install dependencies
```bash
pip install -r requirements.txt
```

### Step 3: Run the Python notebook
Open `notebooks/Customer_Shopping_Behavior_Analysis.ipynb` and run all cells to clean the data, engineer features, and generate the EDA plots.

### Step 4: Load data into SQL
1. Create a database in PostgreSQL/MySQL/SQL Server.
2. Set your connection details as environment variables (never hardcode credentials) — the notebook includes ready-to-edit connection cells for all three databases.
3. Run `sql/customer_behavior_sql_queries.sql` against the loaded table.

### Step 5: Open the Power BI dashboard
Open `dashboard/customer_behavior_dashboard.pbix`, connect it to your SQL database, and refresh.

---

## 📊 Key Business Questions Answered
- Who are the highest-value customers, and what drives their purchases?
- Do subscribers spend more than non-subscribers, and by how much?
- Which products are most discount-dependent vs. highest-rated?
- How does shipping type relate to purchase amount?
- How should customers be segmented (New / Returning / Loyal), and what's the revenue mix by age group?

Full write-up: [`docs/Customer Shopping Behavior Analysis.pdf`](docs/Customer%20Shopping%20Behavior%20Analysis.pdf)
Business framing: [`docs/Business Problem Document.pdf`](docs/Business%20Problem%20Document.pdf)
Presentation: [`docs/Customer-Shopping-Behavior-Analysis.pptx`](docs/Customer-Shopping-Behavior-Analysis.pptx)

---

## 💼 Skills Demonstrated
Data Cleaning · Feature Engineering · Exploratory Data Analysis · SQL (CTEs, window functions, conditional aggregation) · Dashboard Development · Business Insight Generation · Data Storytelling

---

## 👨‍💻 Author
**Anurag Kumar Singh**
Aspiring Data Analyst skilled in Python, SQL, and Power BI.
Passionate about building real-world analytics projects and solving business problems using data.

**GitHub:** https://github.com/Anurag-M1

---

## ⭐ Support
If you found this project helpful, star ⭐ the repo, fork it, or share it with others.
