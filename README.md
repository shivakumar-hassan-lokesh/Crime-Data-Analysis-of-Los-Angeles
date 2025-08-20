<img width="1105" height="770" alt="Screenshot 2025-08-20 at 5 50 09 PM" src="https://github.com/user-attachments/assets/09427d47-bc3c-41e6-ae3e-a09fd5b2e488" />

## 📌 Project Overview
This project explores and analyzes crime data from **Los Angeles (2020–Present)** to uncover patterns, trends, and insights.  
The analysis involves **data cleaning, exploratory data analysis (EDA), demographic insights, anomaly detection, and forecasting** using ARIMA.  

The goal is to understand **crime trends** over time, identify **regional hotspots**, and provide **predictive insights** to assist policymakers and law enforcement.


## 📂 Dataset
- Source: **Crime Data from 2020 to Present (Los Angeles)**  
- Size: ~982,000 records  
- Key Columns:  
  - `DATE OCC` – Date of occurrence  
  - `AREA NAME` – Region of crime  
  - `Crm Cd Desc` – Crime description  
  - `Vict Age`, `Vict Sex`, `Vict Descent` – Victim demographics  
  - `LAT`, `LON` – Location coordinates  


## ⚙️ Project Workflow
### 1. Data Acquisition & Inspection
- Loaded dataset (`CSV`) into Pandas  
- Inspected data types, columns, and first rows  

### 2. Data Cleaning
- Converted date columns to datetime format  
- Removed duplicates  
- Filled missing values (categorical → `"Unknown"`, numeric → median)  
- Standardized numeric/categorical types  

### 3. Exploratory Data Analysis (EDA)
- **Overall Trends** → Crimes per year  
- **Seasonal Patterns** → Crimes by month  
- **Crime Types** → Top 10 most frequent crimes  
- **Regional Differences** → Crimes by LA regions  
- **Day of the Week** → Distribution of crimes (weekdays vs weekends)  
- **Heatmaps** → Crime frequency by day & hour  

### 4. Advanced Analysis
- **Outliers & Anomalies** → Detected unusual spikes in crime counts & victim ages  
- **Demographics** → Analysis by age, sex, and descent groups   
- **Forecasting (ARIMA)** → Predicted crime trends for next 12 months  


## 📊 Key Insights
1. Crimes peaked and dropped across years, with a sharp decline during the **COVID-19 lockdown**.  
2. **Summer months** show higher crime activity compared to winter.  
3. **Theft, burglary, and vehicle-related crimes** are most common.  
4. **Central & Hollywood** are major hotspots.  
5. Crimes are **more frequent on weekends**.  
6. Victims are mostly **20–40 years old**, with outliers in young and elderly groups.  
7. ARIMA forecasting shows a **gradual rise in crime activity** with seasonal fluctuations.  


## 📈 Visualizations
- Crimes per Year (Bar Chart)  
- Crimes per Month (Line Plot)  
- Top 10 Crime Types (Bar Chart)  
- Crimes by Region (Horizontal Bar Chart)  
- Crimes by Day of Week (Bar Chart)  
- Heatmap of Crimes by Day & Hour  
- Forecasting (ARIMA Predictions)  


## 🛠️ Tech Stack
- **Python** (Pandas, NumPy)  
- **Visualization**: Matplotlib, Seaborn  
- **Time Series Forecasting**: ARIMA (statsmodels)  
- **Jupyter Notebook** for workflow  


## 🚀 How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/crime-data-analysis.git
   cd crime-data-analysis
