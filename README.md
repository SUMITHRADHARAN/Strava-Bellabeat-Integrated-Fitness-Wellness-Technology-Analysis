# Strava & Bellabeat: Wellness Technology Consumer Analysis

<p align="center">
  <img src="https://i0.wp.com" width="200" alt="Strava Logo">
</p>

## 📌 Project Overview
This project provides a comprehensive end-to-end analysis of smart device fitness data. By integrating **SQL** for data engineering, **Python** for deep-dive EDA, and **Power BI** for executive-level visualization, the analysis identifies key correlations between daily activity (steps, calories) and physiological outcomes (BMI, Heart Rate, Sleep) to provide actionable growth strategies for wellness technology.

---

## 🗃️ Datasets Used
The analysis utilized the following 18 datasets, integrated and cleaned via SQL:

*   **dailyActivity_merged.csv**
*   **dailyCalories_merged.csv**
*   **dailyIntensities_merged.csv**
*   **dailySteps_merged.csv**
*   **heartrate_seconds_merged.csv**
*   **hourlyCalories_merged.csv**
*   **hourlyIntensities_merged.csv**
*   **hourlySteps_merged.csv**
*   **minuteCaloriesNarrow_merged.csv**
*   **minuteCaloriesWide_merged.csv**
*   **minuteIntensitiesNarrow_merged.csv**
*   **minuteIntensitiesWide_merged.csv**
*   **minuteMETsNarrow_merged.csv**
*   **minuteSleep_merged.csv**
*   **minuteStepsNarrow_merged.csv**
*   **minuteStepsWide_merged.csv**
*   **sleepDay_merged.csv**
*   **weightLogInfo_merged.csv**

🔗 **Dataset Source:** [FitBit Fitness Tracker Data (Kaggle)](https://www.kaggle.com)

---

## 🛠️ Technical Stack
*   **Data Engineering:** SQL (Data Cleaning, Schema Design, Multi-table Joins)
*   **Data Analysis:** Python (Pandas, NumPy, Seaborn, Matplotlib)
*   **Data Visualization:** Power BI (DAX, Interactive Dashboards)

---

## 📂 Project Structure & Quick Links
Access the core project files directly via the links below:

*   **📊 Power BI Dashboard:** [Strava_Fitness-PBI.pbix](./Strava_Fitness-PBI.pbix)
*   **🐍 Python Analysis (EDA):** [Strava_fitness_PYTHON Code.ipynb](./Strava_fitness_PYTHON%20Code.ipynb)
*   **🗄️ SQL Scripts:** [Strava_fitness-SQL.sql](./Strava_fitness-SQL.sql)
*   **📈 PDF Report:** [Strava_Fitness-PBI%20Dashboard.pdf](./Strava_Fitness-PBI%20Dashboard.pdf)
*   **📑 Master Dataset:** [Strava Full Merged Data.csv](./Strava%20Full%20Merged%20Data.csv)

---

## 📂 Project Modules

### 1. SQL: Data Foundation & Integration
Built a robust database architecture to handle disparate tables (activity, heart rate, sleep, etc.).
*   **Integration:** Merged daily and time-based metrics into a master `StravaFullMergedData` table.
*   **Cleaning:** Standardized data types, handled null values, and removed duplicates across time-series datasets.
*   **Analysis:** Identified top performers and analyzed sedentary patterns vs. high-intensity peaks.

### 2. Python: Exploratory Data Analysis (EDA)
Performed deep-dive analysis to uncover hidden correlations in user movement.
*   **The "V-Dip" Trend:** Discovered that Sundays represent the weekly low for active minutes, highlighting a key retention risk.
*   **Sedentary Load:** Identified a 68.8% average sedentary load across the user base.
*   **Visualizations:** Created activity heatmaps and correlation matrices mapping steps, distance, and calorie burn.

### 3. Power BI: Executive Dashboard
Developed an interactive dashboard focusing on health KPIs and physiological outcomes.
*   **Key KPIs:** BMI (Avg. 25.21), Heart Rate (Avg. 78.60 BPM), and Sleep Duration (Avg. 419 mins).
*   **Advanced DAX:** Calculated total aggregations for 41,709K steps and 247K total calories.
*   **Visual Insights:** Revealed that **96.23%** of the user base is classified as "Overweight" with significant activity volume decline from April to May.

---

## 📊 Overall Business Insights
Based on the synthesis of SQL queries, Python EDA, and Power BI visualizations, the following core business trends were identified:

*   **The Sunday Engagement Gap:** Sundays represent the weekly low for activity (6,991 average steps), identifying a critical window for re-engagement marketing.
*   **High Sedentary Load:** Users spend an average of **68.8%** of their day in a sedentary state, highlighting a major market opportunity for "active-break" features.
*   **Physiological Profile:** Over **96%** of the user base is classified as overweight based on BMI data, suggesting that the primary consumer motivation is weight management.
*   **Retention Decay:** There is a **45.7% drop** in data logging consistency between the first and second months, indicating a critical 30-day "honeymoon phase."
*   **Sleep-Activity Correlation:** Users who achieved the 8-hour sleep goal showed a 12% higher step count the following day, proving that recovery features drive activity volume.

---

## 💡 Business Recommendations
*   **"Road to 10k" Challenge:** Personalized coaching to help users bridge the gap from 7,666 average steps to the 10,000-step goal.
*   **Weight Management Tools:** Integrate calorie-deficit trackers specifically for the high-BMI user segment.
*   **Retention Strategies:** Implement push notifications or mid-month "milestone" rewards to combat the engagement drop-off seen in May.
*   **Sleep Hygiene Prompts:** Introduce in-app prompts for consistent sleep schedules to improve recovery.

---

## 🚀 How to Run
1.  **SQL:** Execute scripts in the `/SQL` folder to initialize the database schema and views.
2.  **Python:** Run the `Strava_fitness_PYTHON Code.ipynb` notebook to see the data processing and EDA.
3.  **Power BI:** Open the `Strava_Fitness-PBI.pbix` file to interact with the live report.
