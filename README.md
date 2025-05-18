# 🚖 NYC Taxi Trip Analysis – Data Engineering & BI Dashboard Project

This project presents a comprehensive **end-to-end data analytics pipeline** to explore and visualize trip patterns, fare behavior, and operational metrics across NYC Taxi services using modern data engineering and BI tools.

🔗 **[📁 Full Project Files – Hosted on Box](https://uofi.box.com/s/lbolg9o3o46ybzzd7lhx3kgqcwsx803h)**

---

## 📊 Overview

We engineered a **Lakehouse-based pipeline** using **Microsoft Fabric** and **Dataflow Gen2**, processed 2.1M+ trip records from Parquet format, and built BI dashboards in **Power BI** and **Tableau**.

Due to Fabric ingestion constraints, Tableau was used for more advanced storytelling and interactivity.

---

## 🧠 Objectives

- Design a scalable data processing solution for large Parquet taxi data using **Microsoft Fabric**
- Visualize fare behavior, trip durations, pickup hotspots, and zone-based congestion
- Enable interactivity across boroughs, service zones, taxi types, and rush hours

---

## 🛠️ Tools & Technologies

| Category            | Tools / Tech                                     |
|---------------------|--------------------------------------------------|
| Data Engineering    | Microsoft Fabric, OneLake, Dataflow Gen2         |
| Data Modeling       | Power BI Semantic Model (Star Schema)            |
| BI & Visualization  | Tableau Desktop, Power BI                        |
| Preprocessing       | Data Wrangler, Fabric Pipelines                  |
| Data Format         | `.parquet` → `.csv` (sampled)                    |

---

## 🧱 Project Architecture

1. **Lakehouse Setup** in Microsoft Fabric to manage raw `.parquet` trip data
2. **Dataflow Gen2 Pipeline** for ingestion, transformation, and publishing
3. **Semantic Model Creation** in Power BI with relationships between trip zones, service types, timestamps
4. **Dashboard Design** with calculated metrics, filters, KPI cards, heatmaps, and story-driven interactivity
5. **Final Tableau Dashboard** featuring:
   - Pickup zone heatmaps
   - Rush hour vs non-rush component breakdown
   - Hourly trends by taxi type
   - KPI callouts

---

## 📊 Tableau Dashboard Highlights

- 🔁 **Interactive Filters**: Taxi type, dropoff borough, pickup hour
- 🟨 **Custom Colors**: Borough-coded visuals with a consistent color template
- 🔥 **KPI Tiles**: Most active zone, rush hour % 
- 🧠 **Advanced Charts**: Stacked bars, layered area charts, matrix heatmaps

> The final Tableau dashboard includes 8 visual sheets and covers over **200K+ rows** with cross-filtering enabled across views.

---

## 🧪 Key Features

- Built **custom calculated fields** to derive:
  - Avg fare per mile
  - Peak pickup hour
  - Rush-hour trip ratios
- Created dashboards using **advanced Tableau containers**, dynamic filters, and layout styling
- Used **OneLake + Data Gen Flow 2** for scalable transformations

---

## 📂 Repository Structure

```bash
NYC-Taxi-Trip-Analysis/
├── README.md
├── dashboards/
│   ├── tableau_screenshots/
│   └── dashboard_summary.md
├── docs/
│   └── Final_Project_Report.pdf
├── data/
│   └── sample_trips_1000rows.csv
├── notebooks/
│   └── Fabric_Dataflow_Guide.md
└── links/
    └── Box_Link.txt  # [https://uofi.box.com/s/lbolg9o3o46ybzzd7lhx3kgqcwsx803h]
