# 🚗 CarSalesUK Dashboard

## 📊 Overview
This Power BI dashboard analyzes a mock dataset of **second-hand car sales in the UK**.  
It provides insights into **car prices, mileage, engine sizes, fuel types, and manufacturer trends**, helping users explore how various factors influence vehicle pricing and demand.

---

## 🧩 Steps taken

### 1️⃣ Data Import & Transformation
- Imported dataset from Kaggle: [UK Car Sales](https://www.kaggle.com/datasets/msnbehdani/mock-dataset-of-second-hand-car-sales/data)
- Reviewed and cleaned the data in **Power Query** (no missing values or duplicates found).
- Added two calculated columns:
  - `Price_USD` → Converted from GBP to USD using approximate exchange rate. **_Note -  At the time of doing this project 1 GBP = 1.35 USD_**
  - `Mileage_km` → Converted from miles using the formula:  
    `Mileage_km = Mileage_mi * 1.60934`
- Verified data types and relationships.

### 2️⃣ Data Modelling
- Ensured consistent data formatting for numeric columns.
- Added necessary measures for visualizations (Average Price, Average Mileage, Total Listings).
- Checked that slicers and filters (Manufacturer, Fuel Type, Year) interact correctly.

### 3️⃣ Dashboard Design
Created two Power BI pages for structured storytelling:

#### **Page 1 – Market Overview**
Purpose: Give a high-level understanding of the car market distribution.

**Visuals:**
- **KPI Cards:** Total Listings, Average Price (USD), Average Mileage (KM), Average Engine Size.
- **Bar Chart:** Car count by Fuel Type.
- **Column Chart:** Average Price by Fuel Type.
- **Line Chart:** Average Price by Year of Manufacture.
- **Bar Chart:** Average Mileage by Manufacturer.
- **Treemap:** Market Share by Manufacturer.
- **Slicers:** Manufacturer, Fuel Type, Year.

#### **Page 2 – Price & Brand Insights**
Purpose: Show what drives price differences and brand performance.

**Visuals:**
- **Scatter Plot:** Price (USD) vs Mileage (KM), colored by Fuel Type, bubble size = Engine Size.
- **Column Chart:** Average Price by Manufacturer.
- **Treemap:** Total Revenue by Manufacturer.
- **Stacked Column Chart:** Number of Listings by Manufacturer & Fuel Type.
- **Filters:** Manufacturer, Fuel Type, Year of Manufacture.

---

## 🧾 Dataset
**Source:** [Kaggle – Mock Dataset of Second-Hand Car Sales](https://www.kaggle.com/datasets/msnbehdani/mock-dataset-of-second-hand-car-sales/data)

**Fields Used:**
- Manufacturer  
- Model  
- Engine Size  
- Fuel Type  
- Year of Manufacturer  
- Mileage (miles & km)  
- Price (GBP & USD)

---

## 💡 Key Insights

- Vehicles with **lower mileage and newer manufacturing years** generally command **higher prices**.  
- **Petrol cars** dominate listings, while **Hybrids** have the **highest average prices**.  
- **Porsche** and **BMW** lead in premium pricing; **Ford**, **VW**, and **Toyota** dominate total market share.  
- **Toyota** records the highest total revenue (~$243M USD).  
- **Mileage is inversely correlated with price**, especially for mass-market brands.

---

## ⚙️ Tools Used
- **Power BI Desktop** – Dashboard design & visualization  
- **Microsoft Excel / Power Query** – Data cleaning and transformation  
- **Kaggle Dataset** – Data source  

---

## 🚀 How to Use
1. Clone or download this repository.  
2. Open the `.pbix` file in **Power BI Desktop**.  
3. Interact with filters (Manufacturer, Fuel Type, Year) to explore insights.  
4. View both pages:
   - **Page 1:** Car Market Overview  
   - **Page 2:** Price & Brand Insights  

---

## 🧠 Future Improvements
- Add depreciation and resale value forecasting.  
- Integrate geographic or regional filters (if data available).  
- Include trend comparisons across years and fuel efficiency metrics.  

---

## 📸 Preview
- Page 1: Car Market Overview
  <img width="1400" height="786" alt="image" src="https://github.com/user-attachments/assets/8feff55c-6890-445d-8085-2a945b17142f" />
  
- Page 2: Price & Brand Insights
  <img width="1400" height="786" alt="image" src="https://github.com/user-attachments/assets/4d93e36a-8c2b-4883-8d32-6f62faf7c822" />
  

---

## 🏷️ Author
**Aristo Ayako**  
📧 ayakoaristo9@gmail.com  
🔗 [LinkedIn](https://www.linkedin.com/in/aristo-ayako/) | [Portfolio](https://aristo-portfolio-vert.vercel.app/)

---

## 🪙 License
This project is licensed under the **MIT License** – feel free to use, adapt, and reference for learning or portfolio purposes.
