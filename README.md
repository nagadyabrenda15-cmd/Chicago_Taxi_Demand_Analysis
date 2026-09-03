# Chicago Taxi Demand Analysis — Power BI

## 📊 Project Overview

A collaborative Power BI project analysing Chicago taxi trip data to understand demand patterns, payment behaviour, geographic activity, and company performance.

The project transforms taxi trip records into business insights that can support decisions around vehicle availability, service coverage, curb access, payment planning, and company performance monitoring.

> **Project Type:** Team Project — SOS Squad 4  
> **Tool:** Microsoft Power BI  
> **Analysis Period:** 12–31 December 2023

---

## 🎯 Business Problem

Chicago taxi planners and operators needed a clearer view of:

- When taxi demand is highest
- Where trips are concentrated
- How riders pay and tip
- Which taxi companies have the highest activity
- How operational indicators such as speed and revenue vary

The objective was to turn raw taxi records into clear, decision-focused business insights.

---

## 📁 Dataset & Scope

| Metric | Value |
|---|---:|
| Imported rows | 267,889 |
| Retained taxi trips | 267,884 |
| Error rows removed | 5 |
| Analysis period | 12–31 December 2023 |
| Days covered | 20 |
| Displayed trips | ~268K |
| Revenue analysed | $6.09M |
| Average trip distance | 5.83 miles |
| Recorded card tip rate | 22.97% |

Five imported error messages were removed because they were not taxi trips. Valid trips with missing community-area names were retained in overall totals and revenue calculations but excluded from named-location charts.

---

## 🧹 Data Preparation & Quality

The analysis included several steps to improve consistency and reliability:

- Removed five records confirmed to be error messages rather than taxi trips.
- Retained valid trips even when community-area names were missing.
- Reviewed unusual duration, fare, distance, and speed values where they could affect results.
- Grouped busy periods into defined working periods.
- Grouped fares into meaningful fare ranges.
- Calculated revenue as:

  `Revenue = Fare + Tips + Tolls`

- Calculated card tip percentage as:

  `Card Tip % = Card Tips ÷ Card Fare`

The same trip records were used for revenue, speed, distance, and percentage calculations.

---

## 🏗️ Data Model

The project used a star-schema approach with the taxi trips table as the central fact table.

### Fact Table

**TAXI TRIPS**

Contains one row per taxi trip and supports measures such as:

- Trip count
- Revenue
- Distance
- Average speed

### Dimension Tables

- DATE
- TIME
- PAYMENT
- COMPANY
- LOCATION

The location dimension supports analysis of both pickup and drop-off community areas.

---

## 📈 Key Findings

### 1. Late-Day Demand

Thursday recorded the highest weekday trip volume with **51,606 trips**.

The busiest hour was **17:00**, with **21,245 trips**.

This indicates a strong late-afternoon demand period.

**Business implication:** Operators can consider increasing vehicle and driver availability between **16:00 and 19:00**, with Thursday receiving particular attention.

---

### 2. Near North Side Is a Major Demand Hub

Near North Side ranked first for both:

- Pickup activity
- Drop-off activity

This indicates strong two-way demand rather than only one-directional activity.

**Business implication:** The area is a strong candidate for vehicle staging, curb-access planning, and service monitoring.

---

### 3. Flash Cab Leads Company Activity

Flash Cab recorded approximately **59K trips**, representing **22.16% company market share**.

Additional indicators included:

- Average fare: **$22.08**
- Card tip rate: **22.01%**
- Revenue per mile: **$3.49**

Because smaller companies can produce extreme values from relatively few trips, company performance should be considered alongside trip volume.

---

## 💡 Business Recommendations

### Late-Afternoon Operations

Pilot additional driver and vehicle availability from **16:00–19:00**, prioritising Thursday.

### Near North Side Planning

Develop a staging and curb-access plan while monitoring pickup and drop-off demand by shift.

### Company Performance

Use high-volume operators such as Flash Cab as benchmarks and compare:

- Trip volume
- Market share
- Average fare
- Card tipping
- Revenue per mile

rather than relying on a single KPI.

---

## 📊 Dashboard

The interactive Power BI dashboard will be added to this repository.

It is designed to allow analysis across areas such as:

- Time
- Payment
- Company
- Community area
- Working period

**Dashboard screenshots:** Coming soon

**Power BI file:** Coming soon

---

## 📂 Repository Structure

```text
├── README.md
│
├── presentation/
│   └── Project Presentation
│
├── dashboard/
│   └── Power BI dashboard files and screenshots
│
├── documentation/
│   ├── Data preparation
│   ├── Methodology
│   └── Business insights
│
└── data/
    └── Dataset information

## 👩‍💻 My Contribution

This was a collaborative team project completed as **SOS Squad 4**.

My contribution included:

- Data analysis and interpretation
- Power BI dashboard development
- Data modelling using a star-schema approach
- Developing and reviewing analytical measures
- Identifying key business insights
- Translating findings into business recommendations
- Supporting preparation of the final presentation

The project was completed collaboratively, and this repository presents the team's work while clearly documenting my contribution.

---

## 🛠️ Tools & Skills Demonstrated

**Business Intelligence**
- Microsoft Power BI
- Dashboard Development
- KPI Development
- Business Reporting

**Data Analytics**
- Data Cleaning
- Data Transformation
- Exploratory Analysis
- Data Visualization
- Insight Generation

**Data Modelling**
- Star Schema
- Fact and Dimension Tables
- Pickup and Drop-off analysis
- Consistent KPI calculations

**Business Skills**
- Business Problem Definition
- Analytical Storytelling
- Evidence-based Recommendations
- Decision Support

---

## 📌 Key Project Outcomes

The analysis demonstrated how structured data preparation, data modelling and Power BI visualization can transform taxi trip records into practical business intelligence.

The findings support potential decisions around:

- Vehicle and driver availability
- Demand planning
- Geographic service coverage
- Curb-access planning
- Payment behaviour
- Company performance monitoring

---

## 📊 Dashboard

The interactive Power BI dashboard will be added to this repository.

Dashboard screenshots and the Power BI project file are **coming soon**.

---

## 📄 Project Presentation

The project presentation is available in the [`presentation`](./presentation) folder.

---

## 👥 Team

**SOS Squad 4**

Collaborative Power BI project.
