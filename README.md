
---

## 🔗 Data Source

Sample sales data from:  
[GitHub - sales_100.csv](https://github.com/gchandra10/filestorage/blob/main/sales_100.csv)

---

## ⚙️ Tools & Technologies

- **Python 3.9+**
- **Cassandra (Datastax Astra DB)**
- **pandas** for data processing
- **Git + GitHub** for version control

---

## 🛠️ Medallion Layers

### 🥉 Bronze Table
- Raw data ingested from CSV into Cassandra.

### 🥈 Silver Table
- Cleaned:
  - Removed missing values
  - Validated date formats
  - Removed negative numbers and duplicates
- Loaded into a new table.

### 🥇 Gold Tables
1. **Total Sales by Country**
2. **Top 5 Items by Profit**
3. **Monthly Revenue by Region**

---

## 📸 Output Screenshots

Screenshots of Gold table outputs (using CQL `SELECT *`) are available in the `screenshots/` folder.

---

## 🚀 How to Run

1. Clone this repo
2. Install required packages:  
   `pip install pandas cassandra-driver`
3. Update secure bundle zip path in each Python script
4. Run scripts in order:
