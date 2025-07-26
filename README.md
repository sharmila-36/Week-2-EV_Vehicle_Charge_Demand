# 🚗 EV Adoption Forecasting

This project focuses on analyzing and forecasting the adoption of Electric Vehicles (EVs) in Washington State using vehicle registration data. The insights can guide decision-makers in building sustainable transportation infrastructure and planning EV charging networks.

---

## 📊 Dataset Overview

- **File Name**: `Electric_Vehicle_Population_By_County.csv`
- **Rows**: 20,819
- **Columns**: 10
- **Source**: Washington State Department of Licensing
- **Description**: Contains end-of-month snapshots of registered vehicles (electric and non-electric) across different counties.

### 🔑 Key Columns

| Column Name                    | Description                                                |
|-------------------------------|------------------------------------------------------------|
| `Date`                        | The date (usually end-of-month) of vehicle count snapshot |
| `County`                      | County of registration                                     |
| `State`                       | State of registration (all WA in this dataset)            |
| `Vehicle Primary Use`         | Classification (Passenger, Truck, etc.)                   |
| `Battery Electric Vehicles (BEVs)` | Count of BEVs                                       |
| `Plug-In Hybrid Electric Vehicles (PHEVs)` | Count of PHEVs                               |
| `Electric Vehicle (EV) Total` | Total BEVs + PHEVs                                         |
| `Non-Electric Vehicle Total`  | Total of non-electric vehicles                            |
| `Total Vehicles`              | Sum of EV and Non-EV vehicles                             |
| `Percent Electric Vehicles`   | Share of EVs (in %) among total vehicles                  |

---

## 🧼 Preprocessing Highlights

- Converted `Date` column to `datetime` format
- Filled missing values in `County` and `State` as `"Unknown"` where needed
- Detected and capped outliers in `Percent Electric Vehicles` using IQR
- Ensured numeric columns were properly converted from object types

---

## 🔍 Project Goals

- Analyze electric vehicle adoption trends by county
- Forecast future EV adoption using regression models (e.g., Random Forest, Linear Regression)
- Identify high-growth regions for EV infrastructure planning

---

## 📁 Files

- `Electric_Vehicle_Population_By_County.csv` – Raw dataset
- `ev_analysis.ipynb` – Notebook for preprocessing, visualization, and modeling

---

## 🚀 Next Steps

- Build and evaluate predictive models
- Visualize county-level trends with heatmaps or bar plots
- Suggest policy recommendations based on EV growth trends

---
