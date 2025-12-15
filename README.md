# 📊 Data Leverager – Power BI Power Query Transformation Project

## 📝 Project Overview
**Data Leverager** is an ETL-focused Power BI project that demonstrates real-world
data extraction, cleaning, integration, transformation, and profiling using
**Power BI Power Query Editor only**.

> ❌ No DAX  
> ❌ No Visualizations  
> ✅ Only Data Preparation & Transformation

---

## 🎯 Objective
To simulate a data engineering scenario using Power BI Power Query to extract,
clean, reshape, and combine data from multiple sources while maintaining high
data quality.

---

## 🧰 Tools & Technologies
- Power BI Desktop  
- Power Query Editor (M Language)  
- Excel Files (.xlsx)  
- Web Data (HTML Tables)  

---

## 📂 Data Sources Used
- 🌐 **Web Source**: HTML table (e.g., GDP / COVID / statistics data)
- 📁 **Folder Source**:
  - Sales_Jan.xlsx  
  - Sales_Feb.xlsx  
  - Sales_Mar.xlsx  
- 👥 **Employee Dataset**:
  - EmployeeID  
  - Name  
  - Department  
  - Region  
  - Join Date  

---

## 🔄 ETL Tasks & Transformations

### 1️⃣ Data Extraction
- Loaded HTML table from web
- Loaded multiple Excel files using **Append Queries from Folder**
- Imported Employee data from Excel

---

### 2️⃣ Basic Transformations
- Removed blank rows and columns  
- Promoted first row as headers  
- Renamed columns to meaningful names  
- Changed data types (Change Type with Locale)  
- Removed duplicates  
- Filtered null values  

---

### 3️⃣ Text Transformations
Used Power Query text tools:
- `UPPER()`
- `LOWER()`
- `TRIM()`
- `CLEAN()`
- `REPLACE()`
- `Split Column by Delimiter`

Applied to customer names and address fields.

---

### 4️⃣ Numeric Transformations
- Rounded revenue to 2 decimal places  
- Created calculated column:  
  **Profit = Revenue − Cost**

---

### 5️⃣ Date & Time Transformations
- Extracted Day, Month, Year, Quarter from **Order Date**
- Created **Custom Fiscal Month**
- Calculated **Age** from Birthdate

---

### 6️⃣ Conditional Columns & Indexing
- Created **Sales Category**:
  - High (≥ 10,000)
  - Medium (5,000 – 9,999)
  - Low (< 5,000)
- Added Index Columns:
  - 0-based
  - 1-based

---

### 7️⃣ Pivoting & Unpivoting
- Pivoted monthly sales columns into single column
- Unpivoted back to normalized format

---

### 8️⃣ Merging & Appending
- Merged Sales data with Employee data using:
  - Region / EmployeeID
- Appended Jan–Mar sales using **Append Queries as New**

---

### 9️⃣ Grouping & Aggregation
Grouped data by **Region** and calculated:
- Total Sales
- Average Order Value
- Transaction Count

---

### 🔟 Data Profiling & Quality
Used:
- Column Profile
- Column Distribution
- Column Quality

To:
- Identify missing values
- Detect errors
- Analyze distinct & unique values

---

### 1️⃣1️⃣ Parameters & Source Settings
- Created Parameters for dynamic folder paths
- Managed credentials via Data Source Settings

---

### 1️⃣2️⃣ Refresh Simulation
- Simulated adding new file (Sales_Apr.xlsx)
- Refreshed queries to validate auto-load
- Ensured transformations remained intact

---

## 📦 Deliverables
- Power BI `.pbix` file with all Power Query transformations
- Documentation covering:
  - Data sources
  - Transformations applied
  - Challenges & solutions

---

## ⚠️ Challenges & Solutions

| Challenge | Solution |
|---------|----------|
| Inconsistent columns | Standardized using rename & text tools |
| Data type mismatch | Used Change Type with Locale |
| Missing values | Identified using Column Quality |
| Multiple files | Folder connector with parameters |

---

## 📌 Key Learnings
- Real-world ETL workflow experience
- Strong Power Query transformation skills
- Data quality & profiling techniques
- Scalable design using parameters

---

## 👤 Author
**Data Intern – Janki dholariya**  
Project: *Data Leverager*  
Tool: Power BI (Power Query)