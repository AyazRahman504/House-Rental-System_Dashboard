
# 🏠 House Rental Service Dashboard (India)

### 🔗 [View Dashboard](https://app.powerbi.com/groups/me/reports/8f32a48e-bd61-4b3e-a709-37257e0c4468/ReportSection?experience=power-bi) <!-- Replace with your real Power BI share link -->

---

## 📌 Problem Statement

This project analyzes rental housing data from major Indian cities to help:
- Tenants find suitable homes
- Property owners optimize pricing
- Agents understand market trends

Using Power BI, the dashboard identifies key metrics such as rent amount, furnishing status, city-wise demand, and forecasted trends for upcoming quarters. It provides decision-making support through interactive data storytelling and forecasting tools.

---

## ⚙️ Steps Followed

1. **📂 Load Data**  
   - Two Kaggle datasets: `House_Rent_Dataset.csv` & `_All_Cities_Cleaned.csv`

2. **🧹 Data Cleaning in Power BI**  
   - Renamed columns for clarity (`Posted On` → `Date`)
   - Adjusted column data types (`Rent`, `Size`, `Bathroom` → whole number)
   - Removed redundant columns (e.g., `Area_Locality`, `Property_Type`)
   - Replaced inconsistent values (e.g., `Contact Owner`, `Contact Agent` → `Owner`)
   - Checked for nulls and duplicates

3. **🔗 Merging Datasets**  
   - Combined both datasets based on shared structure

4. **📊 Visualization Design**  
   - Built 2 pages:
     - **General Overview**
     - **Forecast for Next 3 Quarters**
   - Added slicers for `City`, `Seller Type`, `Furnishing`, and `Quarter`
   - Used red, yellow, blue, and orange color-blind–friendly theme

5. **💡 KPI Cards**
   - Total Rent (₹9B), Total Listings (187K), Avg Size (1300 sq ft)

---

## 🧮 DAX Expressions Used

```DAX
-- Total Rent Calculation
TotalRent = SUM(Data[Rent])

-- Average Property Size
AvgSize = AVERAGE(Data[Size])
```

Forecasts were built using Power BI’s **Analytics pane** → **Forecast line** with custom time series.

---

## 📈 Key Insights

1. **🏷️ Market Overview**  
   - ₹9B in total rent  
   - 187,000 listings analyzed  
   - Avg. house size: 1300 sq ft  

2. **🛋️ Furnishing Impact**  
   - Semi-furnished units generated the most revenue (~₹3B)  
   - Unfurnished: ~₹4B | Furnished: ~₹2B

3. **📢 Seller Distribution**  
   - 90%+ of listings posted by agents  
   - Less than 10% by property owners

4. **📆 Monthly Trends**  
   - Peak months: Jan–Mar and Dec  
   - Dip mid-year (May–Sept)

5. **📉 Forecast (Next 3 Quarters of 2023)**  
   - Increase in Q2 (Apr–May)  
   - Projected decline by October

6. **🗺️ City-Level Insights**  
   - Highest rent generated in Mumbai, Delhi, Bangalore  
   - Map-based visualizations highlight demand density

---

## 🖼️ Report Snapshots

### General Analysis Page
![Dashboard 1]([Assets/dashboard%201.png](https://github.com/AyazRahman504/House-Rental-System_Dashboard/blob/main/Assets/dashboard%201.png)

### Prediction of Next 3 Quarters
![Dashboard 2]([Assets/dashboard%202.png](https://github.com/AyazRahman504/House-Rental-System_Dashboard/blob/main/Assets/dashboard%202.png)

---

## 🧑‍💼 Stakeholders Benefited

- **Tenants** → Transparency in pricing and property selection  
- **Property Owners** → Pricing strategy insights  
- **Real Estate Agents** → Understand buyer demand & trends  
- **Regulators** → Oversight via data-driven compliance monitoring  

---

## 📚 Tech Stack

- `Power BI Desktop`
- `Kaggle Datasets`
- `DAX`
- `Data Cleaning & Transformation`
- `Forecasting`
