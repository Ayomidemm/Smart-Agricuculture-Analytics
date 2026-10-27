# 🌾 Smart Agriculture Analytics: From Sensors To Harvest

![Power BI](https://img.shields.io/badge/Power_BI-F2C94C?style=for-the-badge&logo=powerbi&logoColor=black)
![IoT Analytics](https://img.shields.io/badge/IoT_Analytics-00599C?style=for-the-badge)
![Smart Farming](https://img.shields.io/badge/Smart_Farming-27AE60?style=for-the-badge)

An end-to-end data analytics and business intelligence solution built in **Microsoft Power BI** that integrates IoT sensor metrics (NDVI, soil moisture, pH, weather) with crop management practices (irrigation, fertilization, disease tracking) to drive data-informed decisions from sowing to harvest.

---

## 📌 Project Overview

Modern precision agriculture relies heavily on sensor networks and field data to maximize productivity and reduce operational risk. This project aggregates sensor inputs and farming logs into an interactive dashboard that empowers farm managers, agronomists, and agricultural enterprise leaders to:
* Monitor crop health indicators (NDVI, soil moisture, temperature, pH).
* Identify optimal sowing and harvest cycles.
* Compare crop yields across fertilizer formulations and irrigation methodologies.
* Assess regional performance and manage crop disease vulnerabilities.

---

## 🎯 Business & Agronomic Objectives

- **Yield Optimization:** Evaluate average yield benchmarks 4.03K kg/ha across crop varieties (Soybean, Wheat, Maize, Cotton, Rice).
- **Seasonal Cycle Tracking:** Identify peak sowing windows and harvest volume curves across monthly operational cycles.
- **Input Efficiency Analysis:** Determine the ROI and yield contribution of organic vs. inorganic vs. mixed fertilizer treatments.
- **Irrigation Performance:** Measure total yield differences across Sprinkler, Drip, Manual, and Unassisted ("None") irrigation systems.
- **Disease & Regional Monitoring:** Map yield outcomes against disease severity levels across global key growing regions.

---

## 🛠️ Tools & Technologies

- **Microsoft Power BI Desktop:** Interactive dashboard design, custom layout, custom graphics, visual slicers, and bookmarks.
- **DAX (Data Analysis Expressions):** Measures for average metric aggregations (`Average yield_kg_per_hectare`, `Avg NDVI_index`, `Avg soil_moisture_%`, etc.).
- **Power Query:** Data cleaning, type conversion, column transformations, and date table structuring.
- **Data Modeling:** Relationship modeling between IoT sensor telemetry, regional dimension tables, and harvest yield fact data.

---

## 📊 Dashboard Architecture & Key Visuals

### 1. Global Field Metrics (KPI Cards)
* **Average Yield:** $4.03{K kg/ha}$
* **Average NDVI Index:** $0.60$ *(Vegetation vigor indicator)*
* **Soil Health Metrics:** Avg Soil pH (6.52), Avg Soil Moisture (26.75)
* **Environmental Controls:** Avg Temperature (24.68C), Avg Humidity (65.19%), Avg Rainfall (181.69mm), Avg Pesticide Usage (26.59)

### 2. Analytical Visual Modules
* **Sowing-Wise Yield (Area/Line Chart):** Tracks yield potential trajectory across planting months (January to March peak).
* **Yield by Crop Type (Donut Chart):** Proportionate yield contribution among Soybean (21.14%), Wheat (20.25%), Maize (19.78%), Cotton (19.49%), and Rice (19.35%).
* **Harvest-Wise Yield (Distribution Chart):** Life-cycle harvest bell curve spanning April to August, peaking in June (726K).
* **Yield by Fertilizer Type (Donut Chart):** Compares average yield performance between Organic (33.78%), Mixed (33.39%), and Inorganic (32.83%).
* **Yield by Irrigation Type (Column Chart):** Evaluates total production volume across Flood/None ( 0.50M), Sprinkler, Manual, and Drip systems (0.45M).
* **Fertilizer vs. Soil Layering (Ribbon Chart):** Analyzes soil-fertilizer interaction dynamics over categorized scales.
* **Disease Severity Impact (Horizontal Bar Chart):** Compares total yield across disease presence tiers (*Severe*, *None*, *Mild*, *Moderate*).
* **Regional Breakdown Table:** Ranks total yield and average rainfall across key operating regions (Central USA, East Africa, North India, South India, South USA).

---

## 🔍 Analytical Workflow

1. **Data Ingestion:** Imported raw IoT telemetry and farm management records into Power Query.
2. **Data Cleansing & Transformation:**
   * Cleaned sensor data values (`NDVI_index`, `soil_moisture_%`, `soil_pH`).
   * Standardized crop classifications, fertilizer categories, and disease severity ratings.
3. **Data Modeling:** Established unified relationships between temporal data (`harvest_date`, `sowing_date`), regional locations, and numeric measurements.
4. **DAX Metric Development:** Built dynamic measures for multi-field aggregations and regional averages.
5. **Dashboard Development:** Designed a cohesive green/earth-tone themed interface tuned for rapid visual diagnostic scanning.

---

## 📈 Key Insights

* **Optimal Harvest Timing:** Harvest volumes follow a bell curve, peaking in **June (726K total yield)**. Operational planning and logistics should be focused around late Q2.
* **Fertilizer Parity:** Yield per hectare remains virtually identical across Organic ($33.78\%$), Mixed ($33.39\%$), and Inorganic ($32.83%) treatments. Synthetic inputs do not show a significant yield advantage over organic methods.
* **Irrigation Variance:** Fields with Sprinkler and unassisted/flood ("None") irrigation recorded higher overall yields (0.50M) compared to Drip systems (0.45M), suggesting a need to re-evaluate drip emitter application rates during key growing phases.
* **Regional Top Performers:** **Central USA** ($437,426 kg/ha) and **East Africa** (433,690 kg/ha) lead global regional productivity.

---

## 💡 Recommendations for Agronomists & Farm Managers

1. **Input Cost Reduction:** Because inorganic synthetic fertilizers do not yield higher returns than organic or mixed treatments, transition a portion of acreage toward **organic or mixed formulations** to lower input costs without loss of yield.
2. **Irrigation Calibration:** Conduct flow-rate audits on **Drip irrigation** systems to address underperformance relative to sprinkler fields.
3. **Logistics Alignment:** Align harvesting machinery, workforce scheduling, and post-harvest storage infrastructure for the **peak June harvest window**.

---

## ⚠️ Limitations

- **Sensor Granularity:** Analysis assumes uniform sensor calibration across field blocks; sensor drift or localized hardware faults may affect telemetry averages.
- **External Factors:** Macroeconomic market prices for commodities (Soybean, Wheat, Rice, etc.) were not factored into this production-focused dataset.

---

## 🏁 Conclusion

The **Smart Agriculture Analytics** dashboard demonstrates how combining IoT sensor telemetry with traditional farm management metrics creates actionable business intelligence for agriculture. By tracking crop performance from sowing through harvest, farmers and agricultural operators can make data-driven decisions that increase output while conserving resource inputs.
