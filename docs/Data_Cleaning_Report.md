# 🧹 Data Cleaning & Preparation Report  
### E-Commerce Sales Data (2009–2010)

This document describes the complete data cleaning workflow applied to the 2009–2010 e-commerce sales dataset using **Power Query in Power BI**.

---

## 🔍 Raw Dataset Overview
Columns included:
- Invoice  
- StockCode  
- Description  
- Quantity  
- InvoiceDate  
- Price  
- Customer ID  
- Country  

---

# 🧼 Step-by-Step Cleaning Process

## 1️⃣ Correct Data Types
Each column was assigned the correct type:
- `Invoice` → Text  
- `StockCode` → Text  
- `Description` → Text  
- `Quantity` → Whole Number  
- `InvoiceDate` → Date/Time  
- `Price` → Decimal  
- `Customer ID` → Whole Number  
- `Country` → Text  

---

## 2️⃣ Remove Invalid Transactions
To ensure accurate revenue calculation:
- Removed rows where **Quantity ≤ 0** (returns/cancellations)  
- Removed rows where **Price ≤ 0**  
- Filtered out rows with **null or blank Description**  
- Removed rows with missing **Invoice** or **InvoiceDate**

---

## 3️⃣ Standardize Text Columns
Used Power Query’s *Transform → Format* options:
- Trimmed and cleaned whitespace  
- Ensured consistent capitalization where necessary  

---

## 4️⃣ Create Calculated Columns
### **TotalSales**
A new column was created using:

