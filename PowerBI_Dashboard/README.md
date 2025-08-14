## ⚙️ Prerequisites

1. Power BI Desktop  
   – Version 2.146.705.0 or later  
2. Python  
   – Python 3.13.5 installed  
   – Required packages (only for the one Python visual):  
     ```bash
     pip install pandas matplotlib seaborn
     ```  
3. Enable Python scripting in Power BI  
   - File → Options and settings → Options → Python scripting  
   - Point to your local Python installation  

---

## 🐍 Python Visual

This report uses **one** Python‐script visual to render the “Subscription by Previous Contacts” chart. All other visuals are built with DAX measures.

- **Subscription by Previous Contacts**  
  - Script: `seaborn.histplot` of the `previous` column (number of past outreach attempts)  
  - Packages: `pandas`, `seaborn`  

> Tip: If this chart doesn’t render, double-check your Python path in Power BI’s settings and confirm the packages are installed in that environment.

---

## 📊 DAX Measures

All other KPIs and visuals leverage DAX for performance and interactivity:

- **Total Clients Contacted**  
- **Total Subscriptions**  
- **Conversion Rate (%)**  
- **Subscription by Job Type**  
- **Subscription by Education Level**  
- **Monthly Subscription Trends**  
- **Age Distribution (bar chart)**  
- **Marital Status Breakdown**  
- **Housing vs. Personal Loans**  
- **Strategic Recommendations**  

Each measure is defined in the `Model` pane under **New Measure** and optimized for slicer responsiveness.

---

## 🚀 How to Use

1. Clone or download this repo.  
2. Open `bank_marketing_dashboard.pbix` in Power BI Desktop.  
3. Navigate the three report pages:  
   1. **Insights & Narrative**  
   2. **Storytelling & Summary**  
   3. **Strategic Overview**  
4. Interact with slicers (age group, job type, education level, month) and hover over visuals for tooltips.  
