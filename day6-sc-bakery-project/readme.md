# 🍞 Sweet Crust Bakery Project  

<p align="center">
  <img src="https://github.com/najirh/py_bootcampb1_db/blob/main/day6-sc-bakery-project/sc_logo.png" alt="Bakery Image">
</p>  

## 📌 Project Overview  
Sweet Crust Bakery is a **data-driven project** analyzing the **sales performance of a bakery business with 4 stores and 15 products across the USA**.  
The project **automates daily sales reporting**, generates key business insights, and provides visual analytics using **Python, PostgreSQL, and Pandas**.  

## 🛠️ Tools & Libraries Used  
### **Programming & Database:**  
- **Python** – Core programming  
- **PostgreSQL** – Cloud database  
- **pgAdmin 4** – Database management  

### **Data Handling & Processing:**  
- **Pandas** – Data cleaning & transformation  
- **NumPy** – Numeric computations  

### **Data Visualization:**  
- **Matplotlib** – Static charts  
- **Seaborn** – Statistical plots  
- **Plotly/Dash** – Interactive visualizations  

### **Automation & Reporting:**  
- **smtplib** – Email automation  
- **Schedule** – Automated job scheduling  


---

## Requirements (Please remove this section) ❌
# **Sweet Crust Bakery Project - Requirements Document**  

## **📌 Project Overview**  
The **Sweet Crust Bakery Project** is a Python-based **data analytics project** designed for students to work with **realistic sales data** from a bakery business operating in the **USA**. The bakery has **4 stores**, **15 products**, and **5,000+ sales records** from the **last two years**, including sales up to **yesterday**.  

Students will **connect to a PostgreSQL cloud database**, retrieve data, **clean & analyze it**, generate **charts**, and **send automated email reports** to the manager every morning at **8 AM** with key business insights.


## **🔗 Project Workflow**
1. **Connect to Cloud PostgreSQL Database**  
   - Use `psycopg2` to establish a connection.  
   - Fetch **sales, products, and stores** data into Pandas DataFrames.

2. **Data Cleaning & Preprocessing**  
   - Remove **duplicate entries**.  
   - Handle **missing values** (e.g., fill in missing prices, replace NaN).  
   - Convert **date fields** to `datetime` format.  
   - Standardize **column names**.

3. **Data Analysis & Visualization**  
   - Generate insights using `matplotlib` & `seaborn`.  
   - Key charts include:  
     ✅ **Sales Trends Over Time**  
     ✅ **Top-Selling Products & Stores**  
     ✅ **Monthly & Yearly Sales Comparison**  
     ✅ **Sales Distribution by Store & Product Category**  
   - Save and **email the charts** to the **manager**.

4. **Business Problem Solving**  
   - Find **bestselling products & stores**.  
   - Identify **low-performing items** & potential discounts.  
   - Understand **seasonal sales patterns**.  
   - Check **monthly revenue growth** trends.

5. **Automated Daily Sales Report (8 AM Job)**  
   - **Schedule a Python script** using `schedule` or `cron`.  
   - Send an **email report** to the **manager** with:  
     ✅ **Total sales of yesterday**  
     ✅ **Total sales of current year & last year**  
     ✅ **Best-selling stores & products of the year**  
     ✅ **Key insights & recommendations**  

---

## **📂 Project Requirements**
### **📌 1. Technologies & Libraries**  
- **Python 3.8+**  
- **PostgreSQL (Cloud Database)**  
- **pandas** (Data handling)  
- **psycopg2** (PostgreSQL connection)  
- **matplotlib, seaborn** (Charts & graphs)  
- **schedule** (Automated email scheduling)  
- **smtplib** (Sending emails)

### **📌 2. PostgreSQL Database Schema**  
#### **🛒 Stores Table**
| store_id | store_name       | location      | established_year |
|----------|-----------------|--------------|------------------|
| 1        | Sweet Crust NYC  | New York, NY | 2015             |
| 2        | Sweet Crust LA   | Los Angeles, CA | 2018         |
| 3        | Sweet Crust SF   | San Francisco, CA | 2020      |
| 4        | Sweet Crust TX   | Houston, TX  | 2019             |

#### **🥐 Products Table**
| product_id | product_name      | category     | price  |
|------------|------------------|-------------|--------|
| 1          | Chocolate Muffin | Muffins      | 3.50   |
| 2          | Blueberry Scone  | Scones       | 4.00   |
| 3          | Croissant        | Pastry       | 3.75   |
| ...        | ...              | ...         | ...    |

#### **📊 Sales Table (5,000+ Records)**
| sale_id | sale_date  | store_id | product_id | quantity | total_price |
|---------|-----------|----------|------------|----------|-------------|
| 1       | 2023-01-15 | 2        | 5          | 4        | 14.99       |
| 2       | 2024-06-20 | 3        | 8          | 2        | 9.99        |
| ...     | ...       | ...      | ...        | ...      | ...         |

---

## **📩 Automated Email Report (Daily 8 AM)**
### **Subject:** 📊 Sweet Crust Bakery - Daily Sales Report (YYYY-MM-DD)
### **Body:**  

📅 **Sales Summary (Yesterday - YYYY-MM-DD)**  
- 📈 **Total Sales:** $XXX.XX  
- 🏆 **Best Store:** Sweet Crust NYC ($XX.XX)  
- 🍩 **Top Product:** Chocolate Muffin (XX units)  

📊 **Yearly Comparison**  
- **Total Sales in 2024:** $XX,XXX  
- **Total Sales in 2023:** $XX,XXX  
- 🔥 **Growth Rate:** XX%  

📢 **Key Insights:**  
✅ Bestselling store: `Sweet Crust NYC`  
✅ Bestselling product: `Chocolate Muffin`  
✅ Slowest-selling product: `Gluten-Free Bread`  

📎 **Attached Graphs:**  
📌 Monthly Sales Chart 📌 Bestselling Products 📌 Store Performance  

📧 **This report was auto-generated.**  

---

## **⏳ Project Deliverables**
✅ **Database Setup & Connection Script**  
✅ **Data Cleaning & Transformation Code**  
✅ **Exploratory Data Analysis & Insights**  
✅ **Business Solutions & Recommendations**  
✅ **Automated Email Reports**  
✅ **Documentation & Final Report**  

---

### **🚀 Next Steps**
1. **Set up PostgreSQL Cloud Database.**  
2. **Write Python scripts to retrieve & clean data.**  
3. **Generate charts & insights using matplotlib/seaborn.**  
4. **Schedule an email automation job for 8 AM reports.**  
5. **Solve key business problems.**  


### **📌 How to Mention This Project in Resume**  

- **Developed** an **end-to-end data analytics pipeline** for a bakery business using **Python, PostgreSQL, and Pandas** to analyze sales from the last two years.  
- **Designed** and **implemented** data cleaning processes to remove duplicates, handle missing values, and standardize sales data, improving data quality.  
- **Created** visual reports using **Matplotlib and Seaborn** to identify best-selling products, store performance, and sales trends over time.  
- **Automated** daily email reports using **Python and SMTP** to send key business insights, boosting decision-making efficiency.  
- **Gained hands-on experience** in **SQL queries, data visualization, automation, and business intelligence**, applying real-world problem-solving skills.  
---

