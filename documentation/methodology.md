# Analysis Methodology

## Objective

The analysis was designed to understand Chicago taxi demand and identify patterns that could support operational and business decisions.

The analysis focused on four main areas:

- Taxi demand
- Payment behaviour
- Geographic activity
- Company performance

## Data Model

The Power BI model follows a **star-schema approach**.

### Fact Table

**TAXI TRIPS**

Contains the individual taxi trip records used for analysis.

Key measures include:

- Trip count
- Revenue
- Trip distance
- Average speed

### Dimension Tables

The model uses dimensions for:

- Date
- Time
- Payment
- Company
- Location

The location dimension supports analysis of both **pickup areas** and **drop-off areas**.

## Key Measures

The analysis used consistent calculations across the dashboard.

### Trip Count

The number of retained taxi trip records.

### Revenue

Revenue was calculated as:

**Fare + Tips + Tolls**

### Average Trip Distance

Total trip distance was analysed against the number of trips to understand typical journey length.

### Card Tip Percentage

Card tipping was measured using:

**Card Tips ÷ Card Fare**

### Revenue per Mile

Revenue was compared with trip distance to provide a measure of revenue generated relative to distance travelled.

## Analytical Views

The dashboard examined the data from several perspectives.

### Time Analysis

Trips were analysed by:

- Day of the week
- Hour of the day
- Working periods

This helped identify periods of higher taxi demand.

### Location Analysis

Pickup and drop-off activity was compared to identify areas with strong taxi movement and potential two-way demand.

### Payment Analysis

Payment types, fares and card tipping behaviour were analysed to understand customer payment patterns.

### Company Analysis

Taxi companies were compared using measures such as:

- Trip volume
- Market share
- Average fare
- Card tip rate
- Revenue per mile

## Business Interpretation

The analysis focused not only on numerical results but also on what those results could mean for taxi operations.

Examples include:

- Planning vehicle availability during high-demand periods
- Understanding important pickup and drop-off areas
- Monitoring company performance
- Supporting operational planning

## Important Limitation

High trip volume does not automatically prove that traffic congestion caused lower speeds. The dashboard results show patterns in the available taxi records and should be combined with other information before making operational decisions.
