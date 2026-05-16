# ✈️ Aviation Operational Performance Analysis (2019–2020)

A data analytics capstone project examining U.S. airline delay patterns, cancellations, and operational disruptions using Power BI and a dataset of nearly 1 million arrival flights.

---

## 📋 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Overview](#dataset-overview)
- [Tools](#tools)
- [Data Preparation](#data-preparation)
- [Key Findings](#key-findings)
  - [Delay Causes](#delay-causes)
  - [Airport Performance](#airport-performance)
  - [Airline Performance](#airline-performance)
- [Dashboard Preview](#dashboard-preview)
- [Strategic Recommendations](#strategic-recommendations)
- [Business Impact](#business-impact)
- [Project Report](#project-report)

---

## 📌 Project Overview

Airline delays cost the aviation industry billions of dollars annually and significantly impact passenger experience. This project analyses arrival flight data across multiple U.S. airports and carriers between 2019 and 2020 to uncover the primary drivers of operational disruptions.

The analysis covers:
- Delay causes and their relative contributions
- Airport-level congestion and performance
- Airline-level operational efficiency
- Year-on-year performance trends (2019 vs 2020)

> **Group 28 Capstone Project | Data Analytics Programme**

---

## 📊 Dataset Overview

| Metric | Value |
|---|---|
| Total Arrival Flights | 997,120 |
| Flights Delayed (≥15 min) | 170,477 |
| Cancelled Flights | 9,643 |
| Diverted Flights | 1,925 |
| Period Covered | 2019 – 2020 |

### Columns in the Dataset

| Column | Description |
|---|---|
| `year` | Year of flight record |
| `month` | Month of flight record |
| `carrier` | Airline carrier code |
| `carrier_name` | Full carrier name |
| `airport` | Airport code |
| `airport_name` | Full airport name and location |
| `arr_flights` | Total arrival flights |
| `arr_del15` | Flights delayed 15+ minutes |
| `carrier_ct` | Count of carrier-caused delays |
| `weather_ct` | Count of weather-caused delays |
| `nas_ct` | Count of NAS (National Airspace System) delays |
| `security_ct` | Count of security delays |
| `late_aircraft_ct` | Count of late aircraft delays |
| `arr_cancelled` | Cancelled flights |
| `arr_diverted` | Diverted flights |
| `arr_delay` | Total arrival delay minutes |
| `carrier_delay` | Carrier delay minutes |
| `weather_delay` | Weather delay minutes |
| `nas_delay` | NAS delay minutes |
| `security_delay` | Security delay minutes |
| `late_aircraft_delay` | Late aircraft delay minutes |

---

## 🛠️ Tools

| Tool | Purpose |
|---|---|
| **Power BI** | Dashboard development and interactive visualisation |
| **Microsoft Excel** | Initial data exploration and cleaning |
| **DAX** | Custom measures and calculated columns in Power BI |

---

## 🔧 Data Preparation

The following steps were carried out to prepare the dataset for analysis:

1. **Data Inspection** – Reviewed column types, null values, and summary statistics
2. **Data Cleaning** – Validated delay minute columns and ensured consistency across carrier and airport records
3. **Feature Engineering** – Derived delay rate (%) and total delay minutes per carrier/airport for ranking analysis
4. **Aggregation** – Grouped records by carrier, airport, year, and month for trend and comparative analysis
5. **Dashboard Modelling** – Structured data relationships in Power BI for cross-filtering across visuals

---

## 🔍 Key Findings

### Delay Causes

Total delay minutes by cause across the full dataset:

| Delay Type | Total Minutes |
|---|---|
| ✈️ Late Aircraft | 4,200,591 |
| 🏢 Carrier | 3,826,943 |
| 🛫 NAS (Airspace) | 2,505,844 |
| 🌦️ Weather | 593,688 |
| 🔒 Security | 18,055 |

**Late aircraft delays** are the single largest contributor, reflecting delay propagation — where a late-arriving aircraft causes delays on its next scheduled departure. **Carrier delays** (crew scheduling, ground ops, servicing) rank second, while **weather and security delays** are comparatively minor.

---

### Airport Performance

- High-traffic hub airports experience the most operational delays due to congestion and high turnaround demand.
- **Dallas/Fort Worth International Airport** recorded approximately **130,007 minutes** of total delay — one of the highest in the dataset.
- Delay propagation is particularly severe at hub airports where gate availability directly affects subsequent departures.

---

### Airline Performance

| Airline | Total Delay Minutes (approx.) |
|---|---|
| SkyWest Airlines | ~1,804,000 |
| Southwest Airlines | ~1,396,083 |

- **SkyWest Airlines** recorded the highest total delay minutes, partly because regional carriers operate high volumes of feeder flights with tighter turnarounds.
- Airline performance is heavily influenced by aircraft utilisation efficiency, crew scheduling quality, and real-time operational monitoring.

---

## 📸 Dashboard Preview

> *Power BI dashboard screenshots — add images here after exporting from Power BI Desktop.*

To view the interactive dashboard, download the `.pbix` file and open it in [Power BI Desktop](https://powerbi.microsoft.com/desktop/) (free).

📥 **[Download Dashboard (.pbix)](./Capstone_Project_Group_28_Aviation.pbix)**

---

## 💡 Strategic Recommendations

1. **Predictive Analytics** — Deploy predictive models to anticipate weather and congestion-driven disruptions before they cascade.
2. **Schedule Buffers** — Incorporate time buffers in aircraft rotation planning to reduce the knock-on effect of late aircraft delays.
3. **Disruption Recovery** — Strengthen irregular operations (IROPS) procedures to recover faster when disruptions occur.
4. **ATC Coordination** — Increase collaboration with air traffic management to ease congestion at high-traffic corridors.

---

## 💼 Business Impact

Improving on-time performance generates direct business value:

- 📈 Higher passenger satisfaction and loyalty
- 💰 Reduced operational costs (crew overtime, fuel burn, rebooking)
- 🔄 Better aircraft utilisation across the network
- 🏆 Stronger brand reputation in a competitive market

Even small reductions in average delay minutes can translate to significant savings across a large flight network.

---

## 📄 Project Report

The full written report is available here:

📥 **[Download Full Report (PDF)](./Capstone_Project_Group_28_Aviation_Report.pdf)**

---

## 👥 Contributors

- **Shaibu Atekojo Wisdom** — [@wisdom223](https://github.com/wisdom223)
- Group 28 Members (TechCrush BootCamp)

---

*Dataset covers U.S. arrival flight records from the Bureau of Transportation Statistics (BTS), 2019–2020.*
