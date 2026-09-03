# Data Preparation

## Overview

The Chicago Taxi dataset was prepared in Power BI before analysis and visualization.

The objective was to ensure that the dashboard used consistent and reliable records for measuring taxi demand, revenue, payment behaviour, location activity and company performance.

## Dataset

- Imported rows: 267,889
- Retained taxi trips: 267,884
- Error rows removed: 5
- Analysis period: 12–31 December 2023
- Number of days: 20

## Data Cleaning

Five imported records contained error messages rather than valid taxi trip information. These records were removed from the analysis.

The remaining taxi trip records were retained for analysis.

Records with missing community-area names were still included in overall trip and revenue calculations. However, they were excluded from named location charts where an identifiable area was required.

## Data Quality Checks

The data was reviewed for unusual values involving:

- Trip duration
- Fare
- Trip distance
- Speed

These checks helped reduce the risk of unusual records distorting the analysis.

## Business Rules

The analysis used the following rules:

### Revenue

Revenue was calculated as:

**Revenue = Fare + Tips + Tolls**

### Card Tip Percentage

Card tipping was measured as:

**Card Tip % = Card Tips ÷ Card Fare**

### Fare Groups

Fares were grouped into categories ranging from:

- Below $10
- $10–$19
- $20–$29
- $30–$39
- $40–$49
- $50+
- Unknown

### Busy Periods

The analysis paid particular attention to:

- 06:00–09:00
- 16:00–19:00

These periods were used to examine changes in taxi activity throughout the day.

## Result

After preparation, the cleaned dataset provided a consistent foundation for the Power BI data model, dashboard calculations and business analysis.
