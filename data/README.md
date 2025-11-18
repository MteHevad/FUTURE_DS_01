# 📁 Data Folder — 2009–2010 Sales Dataset

This folder contains datasets used in the **Business Sales Dashboard (2009–2010)** project.

---

## 📌 Files

### 1. `ecommerce_2009_2010_raw.csv`
- Original raw E-Commerce Sales Data  
- Contains all transactions recorded during **2009 and 2010**  
- Used as the primary input for Power BI  

### 2. `ecommerce_2009_2010_cleaned.csv` (optional)
- Cleaned dataset exported from Power Query  
- Includes:
  - Removed invalid quantities (negative/zero)  
  - Removed zero or invalid pricing  
  - Removed null descriptions  
  - Added `TotalSales` column (Quantity × Price)  
  - Extracted date fields (Year, Month, MonthName, Quarter)

---

## 📝 Key Data Columns  
| Column | Description |
|--------|-------------|
| Invoice | Unique transaction identifier |
| StockCode | Product code |
| Description | Item description |
| Quantity | Units sold per line item |
| InvoiceDate | Date & time of sale (2009–2010) |
| Price | Price per unit |
| Customer ID | Customer identifier |
| Country | Customer’s country |

---

This folder ensures transparency and reproducibility for all data used in the 2009–2010 analysis.
