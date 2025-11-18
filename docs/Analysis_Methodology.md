# 📊 Analysis Methodology  
### Business Sales Dashboard — E-Commerce Data (2009–2010)

This document explains the analytical approach, data modeling techniques, and DAX measures used to build the final dashboard.

---

# 1️⃣ Data Model
The project uses a **single-table model** (fact table):
- Table Name: **Sales**
- Contains 2009–2010 cleaned transactional data

No relationships or dimension tables were required for Task 1.

---

# 2️⃣ Key Analytical Steps

## 🔹 A. KPI Development
Using DAX, several key metrics were calculated:

```DAX
### **Total Revenue**
Total Revenue = SUM('Sales'[TotalSales])

### **Total Invoices**
Total Invoices = DISTINCTCOUNT('Sales'[Invoice])

### **Total Customers**
Total Customers = DISTINCTCOUNT('Sales'[Customer ID])

### **Average Ordered Value**
Average Order Value = DIVIDE([Total Revenue], [Total Invoices])
