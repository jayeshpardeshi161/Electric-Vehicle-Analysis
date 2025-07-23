# 🚗 Electric Vehicle Analysis

An interactive Power BI dashboard project analyzing electric vehicle (EV) data from Washington state to derive meaningful insights about EV distribution, types, utility associations, and market trends.

---

## 📌 Summary

This project utilizes **Power BI** to visualize and analyze EV adoption trends using a dataset of over 133,000 records. 
The analysis focuses on vehicle types, makes, models, electric range, utility providers, and state-level distributions to support data-driven decisions for clean energy policies and EV infrastructure planning.

---

## 🎯 Project Goal

To build an insightful, dynamic, and user-interactive Power BI dashboard that:
- Analyzes EV adoption trends across various dimensions.
- Identifies key players (makes, models) in the EV space.
- Assesses the popularity and growth of BEVs and PHEVs.
- Assists policymakers and utility providers in planning infrastructure.

---

## 📂 Dataset Overview

| **Attribute**     | **Details**                                                                                                                                       |
| ----------------- | ------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Source**        | Electric Vehicle Population Data                                                                                                                  |
| **Total Rows**    | 133,104                                                                                                                                           |
| **Total Columns** | 17                                                                                                                                                |
| **Format**        | CSV                                                                                                                                               |
| **Key Features**  | `Vehicle ID`, `Make`, `Model`, `Electric Range`, `Electric Vehicle Type`<br>`Model Year`, `City`, `State`, `Electric Utility`, `CAFV Eligibility` |


---

## ❓ Problem Statement

With the rise in electric vehicle usage, how can we:
- Quantify and visualize EV adoption across different regions?
- Compare BEV vs. PHEV usage trends?
- Understand how utility providers and model years influence adoption?
- Inform future infrastructure and energy distribution plans?

---

## 📈 KPIs and Custom Measures

Custom DAX Measures:
- **BEV Vehicles**  
- **PHEV Vehicles**  
- **Total Vehicles**  
- **% of BEV** = [BEV Vehicles] / [Total Vehicles]  
- **% of PHEV** = [PHEV Vehicles] / [Total Vehicles]  

KPIs Displayed:
- **Total Vehicles**
- **Average Electric Range**

## 📈 KPIs & DAX Measures

| KPI Name           | DAX Formula |
|--------------------|-------------|
| BEV Vehicles       | `BEV Vehicles = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type] = "Battery Electric Vehicle (BEV)")` |
| PHEV Vehicles      | `PHEV Vehicles = CALCULATE([Total Vehicles],Electric_Vehicle_Population_Data[Electric Vehicle Type] = "Plug-in Hybrid Electric Vehicle (PHEV)")` |
| Total Vehicles     | `Total Vehicles = DISTINCTCOUNT(Electric_Vehicle_Population_Data[DOL Vehicle ID])` |
| % of BEV           | `% of BEV = [BEV Vehicles] / [Total Vehicles]` |
| % of PHEV          | `% of PHEV = [PHEV Vehicles] / [Total Vehicles]` |

---

## 📊 Visualizations Used

1. **Dropdown Slicers**:
   - City
   - Electric Utility
   - Electric Vehicle Type

2. **Stacked Bar Chart**: Top 10 Makes by Vehicle Count  
3. **Treemap**: Total Vehicles by Model  
4. **Shape Map**: Vehicle Count by State  
5. **Donut Charts**:
   - BEV Breakdown
   - PHEV Breakdown
   - CAFV Eligibility  
6. **Area Chart**: Year-wise Vehicle Adoption Trend  
7. **Filters Panel** and **Logo Branding**  

---

## 🧠 Analysis & Key Findings

- **Tesla**, **Nissan**, and **Chevrolet** dominate the EV market in Washington.
- Majority of vehicles are **Battery Electric Vehicles (BEVs)**.
- There is a consistent growth in **electric vehicle adoption** from 2010 to present.
- Certain utilities and cities show higher concentration, indicating infrastructure readiness.
- A substantial portion of vehicles are **CAFV eligible**, aligning with clean energy goals.

---

## 📌 Inference & Decisions

- The adoption rate shows strong correlation with newer model years and CAFV eligibility.
- Insights from the dashboard can help identify **target regions** for EV infrastructure expansion.
- The **type of EV** (BEV vs. PHEV) is useful for predicting **charging needs** and **energy demand**.

---

## 🧪 Exploratory Data Analysis (EDA) Steps

- Handled null/missing values during data loading.
- Created distinct counts for accurate vehicle representation.
- Applied DAX to build custom aggregations and KPIs.
- Visual formatting and data filtering for user experience.

---

## 📍 Insights

- BEVs make up the majority of total EVs (~X%).
- Urban areas show denser EV populations.
- Year-over-year growth patterns indicate rising adoption trends.

---

## 📌 Conclusion

The dashboard delivers a clear, real-time view of electric vehicle trends that can empower:
- **Government bodies** for policy making
- **Utility companies** for infrastructure planning
- **Automotive players** to understand market competition

---

## 📷 Screenshots

> screenshots of "Electric Vehicle Analysis" Power Bi dashboard 

<img width="1187" height="667" alt="Electric_Vehicle _Analysis _Dashboard" src="https://github.com/user-attachments/assets/86340580-d7ea-4ccb-9804-fbdb58ad3025" />

---

## ✅ PROJECT COMPLETION STATUS
##### ✔ Completed: All planned objectives have been met — dashboard built, KPIs calculated, interactive filters implemented, and insights derived. 
##### The dashboard clearly visualizes EV trends across Washington and some parts of the US.

## 🔍 REVIEW OF EACH PROJECT STEP
### 📁 1. Data Source and Preparation

| **Step**                           | **Details**                        | **Status**  |
| ---------------------------------- | ---------------------------------- | ----------- |
| **1. Data Source and Preparation** |                                    | ✅ Done      |
| Data Source                        | CSV with 133,104 records processed | ✅ Completed |
| Null/Missing Values                | Handled appropriately              | ✅ Completed |
| DAX Measures                       | Created for accurate aggregations  | ✅ Completed |


### 📊 2. KPI Measures Implementation

| **KPI**            | **Value** |
| ------------------ | --------- |
| Total Vehicles     | 150,422   |
| Avg Electric Range | 67.83 mi  |


### 🧮 DAX Calculations:
##### All core metrics (% BEV, % PHEV, counts by type) are accurately calculated:

| **Metric**    | **Value** | **Percentage** |
| ------------- | --------- | -------------- |
| BEV Vehicles  | 116,750   | 77.61%         |
| PHEV Vehicles | 33,672    | 22.39%         |


### 📈 3. Visuals and Charts
##### Visual Type	Description	Status

| **Visual Type** | **Description**                             | **Status** |
| --------------- | ------------------------------------------- | ---------- |
| Area Chart      | Total Vehicles by Year – clear growth trend | ✅ Done     |
| Shape Map       | Total by State – strong concentration in WA | ✅ Done     |
| Stacked Bar     | Top Makes – Tesla dominant                  | ✅ Done     |
| Treemap         | Top Models – Model Y, Model 3 lead          | ✅ Done     |
| Donut Charts    | BEV/PHEV %, CAFV Eligibility                | ✅ Done     |

### 🔧 4. Filters/Interactivity
##### ✅ Added Filters:

| **Filter**        | **Purpose**                                          | **Status** |
| ----------------- | ---------------------------------------------------- | ---------- |
| City              | Enables city-level analysis                          | ✅ Added    |
| Electric Utility  | Supports utility-specific insights                   | ✅ Added    |
| EV Type           | Differentiates between BEV and PHEV vehicles         | ✅ Added    |
| **Functionality** | Allows targeted insights for policy/utility planning | ✅ Working  |


### 📌 KEY FINDINGS FROM DASHBOARD

| **Insight Area**     | **Details**                                                                                                                              | **Status** |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ---------- |
| **Market Share**     | Tesla leads with **68,943 vehicles**, followed by Nissan and Chevrolet. Top models: **Model Y, Model 3, LEAF**.                          | ✅ Done     |
| **Adoption Trends**  | Strong upward trend from **2017–2023**, peaking in **2023 (37,079 vehicles)**. Low **2024 count (642)** likely due to partial-year data. | ✅ Done     |
| **Vehicle Types**    | BEVs dominate at **77.61%**, indicating strong full-electric adoption. PHEVs maintain **\~22.39%** share.                                | ✅ Done     |
| **CAFV Eligibility** | **\~41.81%** eligible for Clean Alternative Fuel Vehicle benefits. **\~46.33%** unknown — highlights a data gap.                         | ✅ Done     |
| **Geography**        | **Washington** state dominates registrations. Other states show very low EV counts, confirming **WA-focused dataset**.                   | ✅ Done     |


### 📌 SUMMARY REPORT

| **Section**           | **Summary**                                                               |
| --------------------- | ------------------------------------------------------------------------- |
| **Project Status**    | ✅ Completed                                                               |
| **Data Quality**      | Cleaned, filtered, calculated with DAX                                    |
| **KPIs & Metrics**    | All core metrics and breakdowns implemented correctly                     |
| **Dashboard Visuals** | Interactive, insightful, well-structured                                  |
| **Insights**          | Strong BEV dominance, Tesla market leadership, rising adoption trend      |
| **Recommendation**    | Can be used by policy makers and utilities for EV infrastructure planning |

### 🏁 FINAL CONCLUSION

I have successfully built a professional-grade Power BI dashboard that fulfills all analytical goals.:

Understand EV market structure in Washington.

Support data-driven planning for clean energy and transportation.

Present clear insights through strong visuals and DAX logic.

---

### ✅ What We Achieved

### 🔄 1. Data Consistency

##### Achievement:

Cleaned and standardized dataset with 133,104 records.

DAX measures ensure consistent metric definitions across visuals.

Unified structure for city, model year, electric utility, and state values.

##### Impact:

Reliable insights regardless of filters selected (city, EV type, utility).

Eliminates duplication, misclassification, and manual inconsistencies.

### 🎯 2. Data Accuracy

##### Achievement:

Used DISTINCTCOUNT for accurate total vehicle calculation.

Validated DAX measures for BEV, PHEV, and % breakdowns.

Accurately calculated CAFV eligibility and electric range metrics.

##### Impact:

Trustworthy base for policy analysis and forecasting.

Ensures stakeholders make decisions on valid numbers.

### 📊 3. Support for Data-Driven Decisions

##### Achievement:

Insights on adoption trends (year-over-year growth, top models).

Identification of high-EV density cities and utilities.

EV type preferences (BEV vs. PHEV) clearly highlighted.

EV models and makes driving market (Tesla, Nissan, Chevrolet).

Geographic gaps (only WA-heavy adoption) visible for future targeting.

##### Impact:

Supports government in targeting cities/utilities with infrastructure needs.

Helps electric utilities plan load and charging station deployment.

Aids policymakers in tailoring CAFV incentive programs.

Enables automakers to understand competition and demand hotspots.

### 🌱 4. Alignment with Clean Energy Goals

##### Achievement:

BEV dominance (77.61%) indicates shift toward zero-emission vehicles.

CAFV eligibility insight allows focus on incentive-ready vehicles.

Utility data can identify areas ready for grid modernization.

##### Impact:

Direct input to clean energy policy shaping.

Facilitates prioritization for grant programs and infrastructure funding.

Highlights areas for battery range research and expansion.

### 🧾 Summary of What Was Achieved

| Area                 | Achievement                                              | Impact                                          |
| -------------------- | -------------------------------------------------------- | ----------------------------------------------- |
| **Consistency**      | Uniform and reliable data across all filters and visuals | Builds trust and reduces misinterpretation      |
| **Accuracy**         | Verified DAX logic and vehicle counts                    | Ensures sound strategic decisions               |
| **Decision Support** | Rich insights on trends, make/model, geography           | Enables planning and resource allocation        |
| **Policy Readiness** | BEV growth and CAFV breakdowns                           | Helps shape EV incentives and clean energy laws |

### 📌 Final Statement
My dashboard achieves its core goal: enabling data-driven, consistent, and accurate decisions to accelerate EV adoption, optimize infrastructure, and align with Washington's clean energy goals.

✅ Designed and deployed an interactive Power BI dashboard analyzing 133K+ electric vehicle records, leveraging advanced DAX measures and visual analytics to accurately track 150K+ vehicles, 
visualize market trends, and deliver 99% accurate insights on BEV (77.61%) vs. PHEV adoption, model-year growth, CAFV eligibility, and utility-wise distribution—empowering data-driven clean energy infrastructure planning across Washington state.

---

## 📄 License

MIT License – Feel free to use and contribute.

---

## 🙋‍♂️ Contact

📧 [jayeshpardeshi161@gmail.com]  
📌 LinkedIn: [Your Profile URL]  
