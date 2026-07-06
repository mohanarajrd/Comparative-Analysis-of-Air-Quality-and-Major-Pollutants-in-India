# 🌍 Comparative Analysis of Air Quality and Major Pollutants in India

An interactive Power BI dashboard that analyzes air quality across India using AQI monitoring data. The project leverages star schema modeling, DAX measures, and dynamic visualizations to compare pollution levels across states, cities, monitoring stations, and pollutant categories, enabling data-driven environmental insights.

---

## 📌 Project Overview

Air pollution is one of the most pressing environmental and public health challenges in India. This project analyzes Air Quality Index (AQI) data collected from monitoring stations across the country to identify pollution hotspots, compare pollutant concentrations, and evaluate air quality trends.

Using Power BI, the dashboard provides interactive insights into pollutant distribution, regional pollution levels, monitoring station performance, and key environmental indicators.

---

## 🎯 Objectives

- Analyze air pollution levels across Indian states and cities
- Compare pollutant concentrations across monitoring stations
- Identify the most polluted cities and regions
- Evaluate pollutant category distribution
- Design an optimized star schema data model
- Build interactive KPIs using DAX
- Support environmental monitoring through dynamic visualizations

---

## 🛠️ Technologies Used

- Power BI
- Power Query
- DAX
- Data Modeling (Star Schema)
- Microsoft Excel

---

## 📂 Dataset Overview

The dataset contains air quality measurements collected from monitoring stations across India.

### Key Attributes

- Country
- State
- City
- Station Name
- Monitoring Board
- Latitude
- Longitude
- Pollutant ID
- Pollutant Category
- Pollutant Minimum
- Pollutant Average
- Pollutant Maximum
- Last Update

---

## 🏗️ Data Model

The dashboard follows a **Star Schema** design.

### Fact Table

**Fact_AQI**

Contains quantitative air quality measurements including:

- Pollutant Average
- Pollutant Minimum
- Pollutant Maximum
- Monitoring Date
- Foreign Keys

### Dimension Tables

#### Dim_Station

Contains:

- Station Name
- Station City
- Monitoring Board
- Latitude
- Longitude

#### Dim_Location

Contains:

- Country
- State
- City

#### Dim_Pollution

Contains:

- Pollutant ID
- Pollutant Category

---

## 🔗 Data Relationships

The Power BI model establishes the following relationships:

- Fact_AQI ↔ Dim_Station
- Fact_AQI ↔ Dim_Location
- Fact_AQI ↔ Dim_Pollution

This model improves query performance while supporting efficient filtering and reporting.

---

## 📊 Key Performance Indicators (KPIs)

The dashboard includes the following KPIs:

- State Average Pollution
- Total Monitoring Stations
- Most Polluted City

These KPIs dynamically update based on user selections.

---

## 📈 Dashboard Visualizations

### Line Chart

**City-wise Pollution Trend**

Shows average pollution levels across cities and highlights pollution hotspots.

### Stacked Bar Chart

**Station-wise Pollution Categories**

Compares pollutant categories across monitoring stations.

### Donut Chart

**Pollutant Distribution**

Displays the proportion of each pollutant category.

### Column Chart

**Average Pollution by City**

Ranks cities based on average pollutant concentration.

### Interactive Slicers

- State
- Pollutant ID

All visuals update dynamically based on slicer selections.

---

## 📊 Analysis Performed

### Descriptive Analysis

- Compared pollution levels across cities
- Identified dominant pollutant categories
- Visualized regional pollution distribution

### Diagnostic Analysis

- Examined pollution sources across monitoring stations
- Compared pollution across geographical regions
- Investigated regional pollution patterns

### Predictive Analysis

- Identified long-term pollution hotspots
- Evaluated recurring pollution trends
- Assessed future environmental risks based on historical patterns

### Prescriptive Analysis

- Highlighted cities requiring immediate intervention
- Recommended focusing on dominant pollutants
- Suggested expansion of monitoring infrastructure
- Supported policy evaluation through scenario analysis

---

## 🔍 Key Findings

- PM2.5 and PM10 were the most dominant pollutants across monitored locations.
- Several cities consistently recorded higher average pollution levels, identifying them as environmental hotspots.
- Pollution levels varied significantly across states and monitoring stations.
- Traffic congestion and industrial activity emerged as major contributors to NO₂ and SO₂ concentrations.
- Dynamic filtering enabled detailed comparison of pollution levels by state, city, station, and pollutant type.
- The star schema data model improved dashboard performance and simplified report development.
- DAX measures provided real-time KPI calculations for better analytical insights.

---

## 📁 Project Structure

```text
Comparative-Air-Quality-Analysis/
│
├── AQI_Dashboard.pbix
├── AQI_Dataset.xlsx
├── README.md
```

---

## ▶️ How to Use

1. Download the repository.
2. Open the `.pbix` file using Power BI Desktop.
3. Refresh the dataset if required.
4. Use the State and Pollutant slicers to interact with the dashboard.
5. Explore KPIs and visualizations to analyze air quality trends.

---

## 💡 Skills Demonstrated

- Power BI
- Data Modeling
- Star Schema Design
- DAX
- Power Query
- Data Visualization
- Dashboard Design
- KPI Development
- Business Intelligence
- Environmental Data Analysis

---

## 📌 Conclusion

This project demonstrates how Power BI can be used to transform raw environmental data into meaningful insights through efficient data modeling, DAX calculations, and interactive visualizations. The dashboard enables comprehensive analysis of air pollution trends, supports environmental decision-making, and showcases practical Business Intelligence techniques for real-world analytical reporting.
