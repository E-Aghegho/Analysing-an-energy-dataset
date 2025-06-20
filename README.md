# Analysing an Energy Dataset (from 2015–2020)

This repository presents a comprehensive, end-to-end analysis of electricity demand, pricing, and environmental factors in Australia, completed by a professional data analyst. The project leverages historical data from AusEnergy (2015–2020) and integrates calendar and climate data to uncover patterns in energy consumption.

The final Excel workbook demonstrates a rigorous data preparation and analysis workflow, complete with visual insights, structured summaries, and presentation-ready deliverables.

---

## 🔍 Analytical Process

### **1. Data Integration & Structuring**
The analyst began by consolidating multiple data sources into a unified workbook:
- Merged **daily electricity demand, RRP, and weather metrics**.
- Integrated **school calendars** and **public holiday data** via lookup functions.
- Organized the workbook with dedicated tabs for raw data and derived features.

### **2. Feature Engineering**
To enrich the dataset:
- Extracted date components: **Day of Week**, **Month**, **Year**, and **Week Number**.
- Added **Holiday** and **School Day** indicators using `VLOOKUP`.
- Calculated a new **Revenue** metric as `Demand × RRP`.

### **3. Formatting for Data Usability**
The dataset was formatted for clarity and exploration:
- Dates were displayed in long, friendly format.
- Demand and revenue values were styled with thousands separators and Australian dollar currency formatting.
- **Conditional formatting** highlighted:
  - Demand levels (green-to-red scale)
  - Outlier RRP values
  - Weather fluctuations using context-aware color scales

### **4. Summary Statistics**
Two sets of summary tables were created:
- **Min, max, and average** values for both **demand** and **revenue**, including associated dates.
- Weekend-specific analysis for **Saturday and Sunday peak demand**.

### **5. Exploratory Time-Series Analysis**
To analyze peak and low demand periods:
- A new tab displayed the **Top 20 and Bottom 20 demand days**, each ranked and annotated.
- A **line chart** traced daily demand fluctuations across the six-year period, making seasonality and long-term trends immediately visible.

### **6. Weather Impact Investigation**
Multiple scatter plots explored the relationship between environmental factors and electricity usage:
- Demand vs. **maximum temperature**, **solar exposure**, and **rainfall**.
- Segmented views plotted demand separately for **school days vs. non-school days** and **holidays vs. working days**.
- **Polynomial trendlines** were used to model nonlinear relationships.

### **7. Time-Based Demand Insights Using Pivot Tables**
To expose consumption trends by time period:
- A **Year-over-Year** pivot table compared monthly demand across all years (excluding incomplete October 2020).
- A pivot chart visualized **weekly demand patterns across days of the week**, with conditional formatting to spotlight high and low demand clusters.

### **8. Report Presentation & Workbook Finalization**
The analyst finalized the deliverable with:
- A clean **cover sheet** introducing the project scope and findings.
- Hidden raw data tabs for a polished presentation.
- Verified chart readability, consistent styles, and workbook usability.

---

## 📂 File Contents

- `AusEnergy Demand Analysis.xlsx`: Complete analysis workbook featuring datasets, calculations, visualizations, and summaries.
- Source files (e.g. `energy_demand.csv`, `holidays.xlsx`) referenced but not included.

---

## 🛠 Tools & Techniques

- Microsoft Excel
  - Functions: `VLOOKUP`, `IFERROR`, `INDEX`, `MATCH`, `MAXIFS`, `TEXT`
  - Pivot Tables & Pivot Charts
  - Conditional Formatting
  - Scatterplots and Polynomial Trendlines

---

## ✨ Key Outcomes

Through this process, the analyst:
- Identified strong temperature-related demand behavior across years.
- Quantified the influence of **holidays** and **school calendars** on consumption trends.
- Delivered a structured, clean, and insightful workbook ready for business presentation or stakeholder review.
