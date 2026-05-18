# Cyclistic Bike Usage Analysis — January to April 2024

This project examines how casual riders and annual members use Cyclistic's bike-share service differently, with the goal of identifying data-driven strategies to convert casual riders into long-term members.

The analysis was originally performed in Google Sheets and documented in a full PDF report. This repository also includes a Python notebook that replicates the analysis using pandas, with structured markdown documentation throughout.

---

## Contents

| File | Description |
|------|-------------|
| `Cyclistic_Bike_Analysis.ipynb` | Python analysis notebook with full code and markdown documentation |
| `Cyclistic_Bike_Data_Analysis.pdf` | Original Google Sheets analysis exported as a detailed report |

---

## Business Objective

Determine how casual riders use Cyclistic bikes differently from annual members to help the marketing team design targeted conversion strategies.

---

## Data Overview

- **Time Period**: January to April 2024
- **Source**: Internal Cyclistic trip records
- **Columns Used**:

| Column | Description |
|--------|-------------|
| `ride_id` | Unique identifier for each trip |
| `rideable_type` | Bike category — classic or electric |
| `started_at` | Trip start timestamp |
| `ended_at` | Trip end timestamp |
| `member_casual` | User type — casual rider or annual member |

**Derived Columns**:

| Column | Method |
|--------|--------|
| `ride_length` | `ended_at` minus `started_at`, in minutes |
| `day_of_week` | Extracted from `started_at` (0 = Monday … 6 = Sunday) |
| `month` | Month name extracted from `started_at` |

---

## Analysis Dimensions

| Dimension | Description |
|-----------|-------------|
| Ride Length vs Bike Type | Average ride duration by user type and bike category, per month |
| Ride Length vs Weekday | Average ride duration by day of the week for each user type |
| Rides by Weekday | Total ride count by user type and day of the week |
| Rides by User Type | Monthly share of rides attributed to casual riders vs members |
| Rides by Bike Type | Bike category preferences (classic vs electric) per user type per month |

---

## Key Findings

### Ride Duration

- Casual riders rode both classic and electric bikes for longer average durations than members in all four months.
- Classic bikes produced longer average rides than electric bikes for both user types, across every month.
- This pattern held consistently without exception from January through April.

### Weekday Patterns

- Casual riders averaged longer ride times than members on every single weekday in every month.
- In March and April, casual riders peaked in average ride length on **Sundays**.
- In January, casual riders peaked on **Mondays**; in February, on **Sundays**.
- Members peaked on **Wednesdays** in January and on **Sundays** in February through April.
- Both user types recorded their shortest average rides mid-week and their longest on weekends (March–April).

### Ride Volume

- Members made more rides than casual riders on every day of the week across all four months.
- Members' ride counts peaked mid-week — **Wednesdays** in March and April.
- Casual riders' ride counts peaked on **Saturdays** in March and April.
- In January and February, both groups concentrated rides mid-week (Wednesdays and Thursdays).

### Ride Share

- Annual members accounted for **more than 75%** of total rides in January and February.
- Casual riders remained **below 30%** of monthly ride volume across all four months.
- The casual rider share increased incrementally each month — lowest in January, highest in April — suggesting seasonal growth as weather improved.

### Bike Type Preferences

- Casual riders preferred electric bikes in January, March, and April; they switched to classic bikes in **February**.
- Members preferred classic bikes in January and February, then shifted to electric bikes in **March and April**.
- In both March and April, members made significantly more rides in both bike categories than casual riders.

---

## Recommendations

- **Weekend and electric bike promotions for casual riders.** Casual riders peak on Saturdays and prefer electric bikes in three of four months. Targeted promotions tied to weekend electric rides offer the highest conversion surface.
- **Usage-based membership prompts.** Casual riders who log three or more rides in a month are strong candidates for membership conversion. Triggered in-app prompts at this threshold could capture riders already habituating to the service.
- **Seasonal fleet and marketing timing.** Casual rider share grows each month from January to April. Spring is the highest-leverage window for membership campaigns. Electric bike availability should scale up on weekends to meet casual demand; mid-week availability should prioritize members.

---

## Summary Report

[Download Full PDF Report](Cyclistic_Bike_Data_Analysis.pdf)

The report includes:
- Data collection and cleaning methodology
- Pivot table visualizations for all five analysis dimensions
- Month-by-month breakdowns for January through April 2024
- Annotated charts comparing casual riders and annual members
