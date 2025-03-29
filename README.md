# 📊 Tableau Dashboard – Visual Analytics Problem Set #7 

This Tableau project includes four diverse dashboards developed for Problem Set #7 in (Visual Analytics). The problems cover business storytelling, KPI tracking with dynamic year-to-year comparison, mapping health data onto human outlines, and building an LOD-driven donor analysis dashboard with parameter interactivity.

---

## 📁 Files Included

| File | Description |
|------|-------------|
| `Problem_Set_7_Dashboard.twbx` | Tableau workbook with all dashboards |
| `screenshots/` *(optional)* | Preview images of each dashboard |

---

## 🟠 Problem 1 – Taste Test Presentation Dashboard

**Objective:**  
Design a clean and presentation-ready dashboard based on a taste test dataset, following *Storytelling with Data* principles.

**Highlights:**
- Visual built in Tableau or Excel
- Embedded into a PowerPoint presentation
- Uses clear comparisons and color to support stakeholder decision-making
- Animation optional (for live delivery)

🎯 **Purpose:**  
Provide clear and concise recommendation based on taste test data and encourage discussion during stakeholder meetings.

---

## 🟢 Problem 2 – KPI Tracker with YoY Comparison (Sample Superstore)

**Dataset:** Sample - Superstore  
**Objective:**  
Create a fully dynamic dashboard that tracks four KPIs (Sales, Profit, Quantity, Discount) with **Year-over-Year (YoY)** comparisons.

🔧 **Techniques Used:**
- Parameter: `Select Benchmark Year` (2022–2024)
- Calculated fields for:
  - CY and PY values using `DATEPARSE`, `DATEADD`, `DATETRUNC`
  - YoY Difference and YoY % Change
- Arrow Symbol Logic (▲ ▼) with color-coded indicators
- Monthly dual-axis line/area charts for each KPI
- Format:
  - Sales & Profit: $K
  - Quantity: #K
  - Discount: % (1 decimal place)
- No tooltips (blank floating object overlay)
- Dynamic dashboard subtitle linked to parameter

🎯 **Result:**  
An executive-level dashboard showing performance deltas and helping leaders identify YoY improvements or declines at a glance.

---

## 🟣 Problem 3 – Injury Heatmap on Human Body Outline

**Dataset:** Injury_Data_Preliminary  
**Objective:**  
Map injury frequency data onto a **front and back human silhouette**, using circle size to indicate injury prevalence.

🔧 **Techniques Used:**
- Scatterplot over custom background images
- Used X/Y coordinates to position injury data
- Size encoded to reflect injury count
- Tooltip includes:
  - Injury location
  - Record count

🎯 **Result:**  
A visually engaging medical mapping dashboard that helps users quickly understand common injury areas.

---

## 🟡 Problem 4 – Donor Drilldown Using LOD (Advancement Dataset)

**Datasets:**  
- Advancement_donations_and_giving_Combined  
- Mapping_US (previous assignment)

**Objective:**  
Enable users to **select a state or Whole Country** via parameter and view:
- Largest donation amount
- Donor name
- Last donation date
- Donor’s major

🔧 **Techniques Used:**
- Parameter: `Get Information from Largest Donor From`
- Filter logic with calculated field `Filter Selection`
- LOD expressions using `{FIXED [State], [Prospect ID] : SUM([Donation Amount])}`
- `ZN()` logic to handle missing values (return 0)
- Map updates highlight the selected state
- Attribute fields shown as text for each metric

🎯 **Result:**  
Interactive donor insights dashboard to support advancement and fundraising decisions across U.S. states.

---

## 🧠 Skills Demonstrated

- Advanced Date & Time calculations in Tableau
- YoY Performance Tracking using Parameters
- Symbol logic (▲ ▼) in calculated fields
- Image-based mapping (X/Y scatterplot over silhouette)
- LOD calculations and conditional data display
- Parameter-based data context switching (state vs national)

---

## 📫 Connect with Me

- 🌐 [LinkedIn – Praneth Nandeesh](https://www.linkedin.com/in/praneth-nandeesh-789038285/)
- 📊 [Kaggle Projects](https://www.kaggle.com/pranethhh)
- ✉️ Email: pranethnandeesh@gmail.com

---

## 📌 License

This project is a student portfolio submission  at Illinois Tech. All dashboards are shared for educational and demonstration purposes only.
