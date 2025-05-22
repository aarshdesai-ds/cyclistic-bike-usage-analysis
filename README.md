# 🚲 Cyclistic Bike Usage Analysis (January–April 2024)

This project explores the behavioral differences between **casual riders** and **annual members** using real-world bike-share data from Cyclistic. The primary business goal is to uncover data-driven insights that can help convert casual riders into long-term members.

All analysis was performed using **Google Sheets**, and findings are documented in a detailed PDF report.

---

## 📘 Summary Report

📄 [**Download Full PDF Summary**](Cyclistic Bike Data Analysis.pdf)

This report contains:
- Data source and cleaning methodology
- Pivot table-driven visual analysis
- Key comparisons (ride length, frequency, bike type)
- Clear month-by-month insights

---

## 🎯 Business Objective

> Help Cyclistic design better membership marketing strategies by understanding how **casual riders use the service differently from annual members**.

---

## 📅 Data Overview

- **Time Period**: January to April 2024
- **Source**: Internal Cyclistic trip data
- **Total Columns Used**:
  - `Ride ID`
  - `Ride Type` (classic or electric)
  - `Start Time`, `End Time`
  - `User Type` (casual or member)

### 🔧 Derived Columns:
- `Ride Length` (calculated as `End Time – Start Time`)
- `Weekday` (0 = Sunday, 1 = Monday, … 6 = Saturday)

---

## 📊 Dimensions Analyzed

| Dimension                | Description                                      |
|--------------------------|--------------------------------------------------|
| Ride Length vs Bike Type | Avg. time by user type and bike type            |
| Ride Length vs Weekday   | Avg. time by day for casuals vs. members        |
| Rides by Weekday         | Count of rides by user type and day of week     |
| Rides by User Type       | Proportion of total monthly rides by user type  |
| Rides by Bike Type       | Preferences for electric/classic per month      |

---

## 📈 Key Insights

1. **Ride Duration**:
   - Casual riders drove both bike types for **longer durations** than members across all months.
   - Classic bikes were consistently used for longer rides by both groups.

2. **Daily Patterns**:
   - Casual riders drove **longer on every weekday** compared to members.
   - Casuals peaked in ride length on **Sundays**, while members were most active on **Wednesdays** and **Sundays**.

3. **Ride Volume**:
   - Members made **more rides every day** than casual riders, across all months.
   - Peak ride counts for members occurred mid-week, while casual riders peaked on **weekends**.

4. **Ride Share**:
   - Casual riders accounted for **<30%** of total monthly rides.
   - Despite longer average rides, casuals contributed fewer total rides each month.

5. **Bike Preferences**:
   - Casual riders **preferred electric bikes** overall, except in **February**, where they chose classic bikes.
   - Members preferred **classic bikes in January and February**, but switched to **electric bikes in March and April**.

---

## 🎯 Recommendations

- 🎯 Focus on converting casual users with targeted weekend and electric bike promotions.
- 📆 Optimize bike availability based on peak weekday patterns.
- 📣 Encourage membership signups through usage-based incentives (e.g., "You rode 3 times this month—unlock more with a membership").

---
