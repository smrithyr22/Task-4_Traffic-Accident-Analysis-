# Task-4_Traffic-Accident-Analysis-

## 🚦Traffic Accident Data Analysis

This repository contains the code, datasets, and visualizations for a comprehensive Traffic Accident Data Analysis project. The goal is to uncover patterns, correlations, and contributing factors behind road accidents using real-world datasets and statistical techniques.

The analysis is based on a cleaned dataset (`traffic_accidents.csv`) and documented in `TASK4.ipynb`.

---

## 🚀Project Goals

Explore and clean traffic accident datasets.

Analyze trends by time, location, weather, road conditions, and vehicle involvement.

Identify high-risk areas and peak accident periods.

Apply statistical and geospatial analysis techniques.

## 📁 Dataset Overview

- **Source**: Internal dataset
- **Original Entries**: 4,320
- **Final Entries (Post-Cleaning)**: 3,262
- **Columns**: 24 variables, including:
  - `crash_date`, `crash_hour`, `crash_day_of_week`, `crash_month`
  - `weather_condition`, `roadway_surface_cond`, `road_defect`, `lighting_condition`
  - `prim_contributory_cause`, `crash_type`, `injuries_total`, etc.



## Data Cleaning
Replaced unknown/unavailable values ('UNKNOWN', 'UNAVAILABLE', etc.) with NaN

Dropped rows with missing values in key columns (weather_condition, lighting_condition, roadway_surface_cond, crash_hour, prim_contributory_cause)

Filled remaining missing values in select features with 'UNKNOWN'

✅Final Dataset is free of null values and ready for analysis 

## 📊 Exploratory Data Analysis
EDA was conducted using Python libraries like Pandas, Seaborn, and Matplotlib, including:

### Weather Conditions
- Most accidents occur in **clear weather**
- Very few under **fog**, **rain**, or **snow**

### Road Surface Conditions
- Crashes mostly on **dry roads**
- **Wet/icy/slushy roads** show minimal representation

### Road Defects
- Majority of crashes involve **no reported defect**
- Minimal contribution from potholes, shoulders, etc.

### Lighting Conditions
- Most crashes occur during **daylight**
- Some in **lighted darkness** (e.g., street-lit areas)

### Time and Day Patterns
- Accidents peak during **morning (7–9 AM)** and **evening (3–6 PM)** commute hours
- **Weekdays**, especially **Friday**, show higher incident frequency

### Crash Types & Injuries
- Dominant crash types: **Rear-end**, **Turning**, **Angle**
- Most crashes involve **0 injuries**
- Fatalities and incapacitating injuries are **very rare**

---

## 🔍 Cause-Based Grouping (Advanced)
Grouped `prim_contributory_cause` by:
- `weather_condition`
- `lighting_condition`

Intended to identify how environmental conditions affect accident causes.

---

## 📊Tools and Technologies 
- Python
- Pandas
- Mathplot
- Seaborn
- Colab

## 📈 Visualizations

The project includes multiple plots using **Matplotlib** and **Seaborn**:
- Count plots for weather, lighting, surface, defect, and crash type
- Time-of-day accident distributions
- Cause-based breakdowns by environmental factors

---

## 🧾 Key Insights

| Factor               | Insight |
|----------------------|---------|
| Weather              | Clear conditions dominate; weather is **not a major contributor** |
| Road Surface         | Mostly dry roads involved; **slippery surfaces are uncommon** |
| Lighting             | Most crashes happen during daylight or well-lit conditions |
| Time of Day          | Rush hours (AM/PM) are highest risk periods |
| Road Defects         | Very few crashes linked to infrastructure issues |
| Injury Severity      | Low injury severity in most cases; majority are non-injury events |
| Crash Types          | Rear-end and turning crashes suggest **driver behavior risks** 
