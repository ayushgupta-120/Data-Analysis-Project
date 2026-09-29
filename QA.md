# Project Questions & Answers (Q&A)
## Crime Data Analysis of India (NCRB 2020)

This document details the key analytical questions explored, the data analysis techniques applied, and the corresponding findings from [`Data_Analysis_Project_with_Python.ipynb`](./Data_Analysis_Project_with_Python.ipynb).

---

### Q1: Which cities in India report the highest overall crime numbers?
- **Objective:** Identify urban centers with the highest total reported offenses to prioritize enforcement and policy focus.
- **Approach:** 
  - Extracted `City` and `Grand_Total` columns from the cleaned dataset.
  - Sorted records in descending order and visualized the top 10 cities using Matplotlib bar charts.
- **Findings:**
  - Metropolitan centers like Delhi report the highest volume of crimes by a significant margin.
  - The top 3 cities account for a substantial proportion of total recorded crimes across all surveyed cities.

---

### Q2: What is the gender distribution among reported criminals?
- **Objective:** Understand gender-wise participation in reported crimes and measure the male-to-female offender ratio.
- **Approach:**
  - Aggregated `Total_Male` and `Total_Female` across all cities.
  - Computed the gender ratio: `Total_Male / (Total_Female + 1e-6)`.
  - Created stacked bar charts for top cities comparing male vs. female offender counts.
- **Findings:**
  - Approximately **80%** of offenders are male, while **~20%** are female.
  - While male offenders heavily dominate overall statistics, female criminal participation shows noticeable spikes in specific cities.

---

### Q3: Which age group accounts for the majority of criminal offenses?
- **Objective:** Identify the age demographic most prone to criminal activity.
- **Approach:**
  - Segmented data across age brackets: `18-30`, `30-45`, `45-60`, and `60+`.
  - Leveraged NumPy array summation (`np.sum`) across all cities.
  - Plotted a proportion pie chart with percentage breakdown.
- **Findings:**
  - Young adults aged **18–30** represent the largest cohort of offenders (~45%+).
  - The **30–45** bracket constitutes the second largest group.
  - Criminal involvement drops progressively in the **45–60** and **60+** demographics.

---

### Q4: What is the extent and impact of juvenile crime?
- **Objective:** Measure juvenile offenses relative to adult offenses and identify high-risk regions.
- **Approach:**
  - Calculated `Juvenile_Percent = (Juvenile_Total / Grand_Total) * 100`.
  - Filtered cities where juvenile crime exceeds 10% of total city crime.
  - Evaluated trend differences between juvenile and adult crimes using multi-line plots.
- **Findings:**
  - Nationally across cities, juvenile offenses account for approximately **6%** of total offenses.
  - Select cities display unusually elevated juvenile rates (>10%), highlighting areas in need of targeted youth rehabilitation and social intervention programs.

---

### Q5: Which cities exhibit high female offender numbers or specific risk criteria?
- **Objective:** Filter and extract subsets of cities with atypical crime profiles.
- **Approach:**
  - Applied Pandas conditional filtering and the `query()` method:
    - Cities with `Total_Female > 1000`.
    - High-density crime cities: `Grand_Total > 10000 and Total_Female > 1000`.
    - Mid-age concentration: `Total_30_45.between(3000, 6000)`.
- **Findings:**
  - Only a select group of major metropolitan hubs cross both thresholds (>10,000 total crimes and >1,000 female crimes), pointing to higher reporting rates and dense populations.

---

### Q6: What statistical correlations exist between male and female crime rates?
- **Objective:** Assess whether female crime correlates with overall male crime volume across cities.
- **Approach:**
  - Constructed a scatter plot comparing `Total_Male` vs `Total_Female` across all cities.
- **Findings:**
  - A positive linear relationship is observed between male and female crime numbers across cities, suggesting that higher general crime rates in large urban hubs scale across both genders rather than being isolated to one demographic.
