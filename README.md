# World Top Restaurants Analysis

**Excel analysis of 50 of the world’s most prestigious restaurants, exploring Michelin ratings, cuisine types, pricing, and chef performance.**

---

## 📂 Project Structure

```
world-top-restaurants-analysis-excel/
│
├── data/
│ ├── raw_data.csv # Original dataset
│ └── cleaned_data.csv # Cleaned & transformed dataset (Power Query)
│
├── report/
│ └── World_Top_Restaurants_Analysis.pdf
│
└── dashboard/
└── world-top-restaurants-dashboard.xlsx # interactive dashboard with slicers and visualizations
```


---

## 🗂 Dataset Overview

This dataset features 50 of the world’s top restaurants, spanning 19 countries across 5 continents. It represents the pinnacle of culinary excellence, from Michelin-starred French institutions to innovative Nordic kitchens and contemporary Latin American cuisine.

**Key columns include:**
- Restaurant_Name  
- City  
- Country  
- Cuisine_Type  
- Michelin_Stars  
- Average_Price_USD  
- Chef  
- Established_Year  
- Seating_Capacity  
- Rating  
- Signature_Dish  
- Years_Operating  
- Price_Category  
- Continent

---

## 🔧 Data Cleaning & Transformation (Power Query)

- Corrected data types for numeric, text, and date fields.  
- Standardized cuisine categories using text trimming and normalization.  
- Imputed missing `Signature_Dish` values with “Not Specified.”  
- Fixed inconsistent country names and added continent mapping.  
- Converted `Michelin_Stars` to numeric and removed redundant `Star_Category`.  
- Standardized chef names (trimmed, proper case).  
- Created derived columns: `Years_Operating` and `Price_Category`.  
- Removed duplicate restaurant entries.  
- Loaded cleaned table into Excel for visualization.

---

## 📊 Key Measures (Power Pivot)

- **Average Price per Star** – Evaluates price-to-prestige ratio.  
- **Top Chef by Average Rating** – Highlights highest-rated chefs globally.

---

## 📈 KPIs (PivotTables)

| KPI | Value |
|-----|-------|
| Total Restaurants | 50 |
| Total Michelin Stars | 96 |
| Average Rating | 4.702 |
| Average Price per Star | 146.39 USD |
| Top Chef by Average Rating | 4.9 |

These KPIs are displayed at the top of the dashboard for immediate insight.

---

## 💡 Business Insights & Visualizations

### 1. Michelin Star Distribution by Continent
- **Pivot:** Rows = `Continent`, Values = `Sum of Michelin_Stars`  
- **Chart:** Column chart  
- **Insight:** Europe dominates with 57 stars, Asia has 17, North America 22, South America 0.

### 2. Average Rating per Cuisine Type
- **Pivot:** Rows = `Cuisine_Type`, Values = `Average of Rating`  
- **Chart:** Stacked column chart  
- **Insight:** French and Italian cuisines consistently achieve top ratings (up to 4.9).

### 3. Average Price per Cuisine Type
- **Pivot:** Rows = `Cuisine_Type`, Values = `Average of Average_Price_USD`  
- **Chart:** Stacked bar chart  
- **Insight:** Avant-Garde, Molecular Gastronomy, and New Nordic are the most expensive cuisines.

### 4. Years Operating vs Michelin Stars
- **Pivot:** Rows = `Years_Operating`, Values = `Sum of Michelin_Stars`  
- **Chart:** Scatter plot  
- **Insight:** Restaurants with 20–36 years of operation tend to earn the most stars.

### 5. Top Restaurants per Continent by Rating
- **Pivot:** Rows = `Continent`, Values = `Max of Rating`  
- **Chart:** Bar chart  
- **Insight:** Top restaurants on each continent achieve ratings around 4.9.

---

## ⚡ Interactivity

Three slicers added for dynamic analysis:  
- Ratings  
- Continent  
- Price Category  

All PivotTables and charts are interactive, allowing users to filter and explore data.

---

## 📝 Summary

This project demonstrates advanced Excel skills including Power Query cleaning, Power Pivot measures, dynamic PivotTables, and interactive dashboards. The PDF report summarizes all KPIs and insights for quick review, while the Excel dashboard provides a fully interactive exploration of Michelin-starred restaurants, cuisine performance, pricing trends, and chef excellence.  

**Folders included:**  
- `data/` – raw and cleaned datasets  
- `report/` – PDF report summarizing analysis and insights  
- `dashboard/` – Excel dashboard with PivotTables, KPIs, charts, and slicers
