# Healthcare Dashboard in Tableau

This project provides a comprehensive Tableau dashboard for visualizing patient data, including patient outcomes, billing, insurance comparisons, length of stay, and trends in admissions. The dashboard is designed to help healthcare administrators and stakeholders identify key trends, improve decision-making, and optimize resource management.

## Project Overview

The dashboard provides insights into:
- Patient outcomes (discharged, deceased, or transferred) by age group and diagnosis type.
- The impact of length of stay on patient outcomes.
- Billing and insurance coverage comparison across age groups and diagnosis types.
- Trends in patient admissions over time.
- Frequency of procedures by diagnosis type and factors contributing to readmission.

The goal is to enable healthcare teams to track important metrics, spot trends, and make data-driven decisions to improve patient care.

## Steps to Create the Dashboard

### Step 1: Define the Objective and Data Insights
The objective is to provide a holistic view of patient data, focusing on key relationships:
1. Patient outcomes by age group and diagnosis type.
2. Impact of length of stay on outcomes.
3. Billing and insurance comparison across age groups and diagnosis types.
4. Admission and discharge trends over time.
5. Procedure frequency by diagnosis type.

### Step 2: Data Preparation
To ensure consistency and comparability, calculated fields were created for:
- **Age Groups** (e.g., 0-17, 18-34, 35-49, 50-64, 65+)
  
Other fields such as patient outcomes, length of stay, billing amount, insurance coverage, and procedures performed were also cleaned and prepared for analysis.

### Step 3: Create Individual Visualizations

#### 1. Patient Outcomes Analysis
- **Chart Type:** Stacked Bar Chart
- **Variables:** Age Group (Columns), Outcome (Rows), Diagnosis Type (Filter)
- **Rationale:** This allows easy comparison of patient outcomes across age groups and diagnosis types.

#### 2. Length of Stay Analysis
- **Chart Type:** Stacked Bar Chart
- **Variables:** Length of Stay (Columns), Readmission Likelihood (Rows), Diagnosis Type (Filter)
- **Rationale:** Visualizes the effect of length of stay on patient outcomes, revealing patterns of extended stays affecting outcomes.

#### 3. Billing and Insurance Comparison
- **Chart Type:** Stacked Bar Chart
- **Variables:** Age Group (Columns), Billing Amount and Insurance Coverage (Rows), Diagnosis Type (Filter)
- **Rationale:** Compares billing amounts versus insurance coverage to identify potential gaps in coverage and out-of-pocket costs.

#### 4. Readmission Prediction
- **Chart Type:** Scatter Plot
- **Variables:** Length of Stay (X-Axis), Readmission Likelihood (Y-Axis), Procedures Performed (Color/Size)
- **Rationale:** Identifies factors contributing to higher readmission rates.

#### 5. Trend Analysis for Admissions
- **Chart Type:** Dual-Axis Line Chart
- **Variables:** Admission Date (Columns), Number of Admissions and Discharges (Rows), Age Group and Gender (Filters)
- **Rationale:** Shows trends in admissions and discharges over time, aiding in resource planning and capacity management.

#### 6. Procedure Frequency Heatmap
- **Chart Type:** Heatmap
- **Variables:** Diagnosis Type (Columns), Procedures Performed (Rows), Frequency (Color Gradient)
- **Rationale:** Provides an overview of common procedures performed for each diagnosis type.

### Step 4: Create the Dashboard
1. **Dashboard Layout:** 
   - Open a new dashboard in Tableau.
   - Set the size to 1200 x 800 pixels (optimized for desktop users).
2. **Add Visualizations:** 
   - Drag the visualizations onto the dashboard canvas, grouping related charts for comparison (e.g., patient outcomes and length of stay).
3. **Filters for Interactivity:** 
   - Add interactive filters for variables like Diagnosis Type and Age Group, allowing users to explore the data in more depth.
4. **Customize Titles and Descriptions:** 
   - Provide clear titles like "Patient Outcomes by Age Group and Diagnosis Type" and "Trends in Admissions Over Time."

### Step 5: Final Touches
- **Test Interactivity:** 
   - Ensure filters and interactive elements work correctly. 
- **Publish the Dashboard:** 
   - Publish the dashboard to **Tableau Public** or **Tableau Server** for sharing with the audience.

## Rationale for Dashboard Design
- **User-Friendly Layout:** The dashboard layout was designed for clarity and ease of comparison across key metrics.
- **Actionable Insights:** Each visualization is designed to provide useful insights, from comparing insurance coverage to identifying readmission risks.

## Dashboard Link
[Access the Tableau Dashboard](https://public.tableau.com/views/Healthcare_17261480238050/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

---

## Requirements
- Tableau Desktop or Tableau Public (latest version).
- Cleaned dataset containing patient age, diagnosis, admission/discharge dates, length of stay, billing, insurance, and procedure data.

## How to Run
1. Open Tableau and load the dataset.
2. Follow the instructions provided above to recreate the visualizations and dashboard.
3. Publish the dashboard to **Tableau Server** or **Tableau Public** for sharing and collaboration.


