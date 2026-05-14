<img width="800" 
height="450" alt="Avalon Hotels Analytics Suite" 
src="https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/assets/avalon-hotels-analytics-suites-logo.png"/>

# Avalon Hotels Booking Analytics Suite

## Executive Summary

The Avalon Hotels Booking Analytics project analyzes hotel reservation patterns, cancellation behavior, and Average Daily Rate (ADR) performance to uncover operational risks and revenue optimization opportunities across resort and city hotels.

The analysis indicates that Avalon Hotels generated approximately **$23.0M in revenue** with an average ADR of **$106.48**, despite maintaining a relatively high cancellation rate of **27.51%**. These metrics highlight the importance of balancing pricing strategy, occupancy management, and cancellation forecasting to sustain operational profitability.

High-risk segments such as Online Travel Agencies (OTAs) and long lead-time reservations contributed disproportionately to cancellations, while direct bookings and shorter lead times demonstrated stronger booking stability.

Additional analysis of ADR trends identified seasonal pricing fluctuations, differences between hotel types, and varying customer value across booking behaviors. Resort hotels generally achieved higher ADR values than city hotels, while booking channels and deposit policies strongly influenced pricing performance.

The dashboards were designed to support hotel executives, revenue managers, and operational teams with interactive KPI monitoring, booking behavior analysis, and data-driven pricing and cancellation reduction strategies.

---

## Project Objectives

The Avalon Hotels Booking Analytics project was conducted to meet the following business objectives: 

- Analyze hotel booking trends to identify seasonal demand patterns and operational booking behavior
- Evaluate cancellation behavior to better understand and reduce revenue loss from canceled reservations
- Investigate Average Daily Rate (ADR) performance to support pricing optimization and occupancy strategies
- Compare hotel types and customer segments to identify high-value and high-risk customer groups
- Develop executive dashboards to support operational monitoring and strategic decision-making

---

## Key Metrics Measured
These key metrics were utilized to evaluate relationships between booking behavior, customer characteristics, operational trends, cancellation patterns, and ADR performance.
| Metric | Description |
|---|---|
| Cancellation Rate | Percentage of bookings canceled before arrival |
| Total Bookings | Total reservation volume |
| Total Cancellations | Number of canceled reservations |
| ADR (Average Daily Rate) | Average revenue earned per occupied room |
| Booking Lead Time | Time between reservation and arrival |
| Market Segment Performance | Booking and cancellation trends across customer groups |
| Customer Type Analysis | Booking and cancellation behavior across customer categories |
| Guest Composition | Analysis of solo travelers, couples, families, and group bookings |
| Hotel Type | Comparison between City and Resort hotels |
| Stay Length | ADR and booking behavior by duration of stay |
---

## Dataset

The Avalon Hotels Analytics Suite uses the Hotel Booking Demand Dataset from Kaggle, containing reservation information for both resort hotels and city hotels between July 2015 and August 2017. The dataset includes approximately 119K hotel booking records and features related to reservation details, customer segmentation, Average Daily Rate (ADR), booking lead time, cancellation behavior, booking channels, deposit policies, and stay duration. A complete data dictionary containing detailed field definitions and variable descriptions is attached below.

[Avalon Hotels Data Dictionary](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/assets/avalon_hotels_data_dictionary.xlsx)

---

## Predictive Analytics & Forecasting

In addition to Tableau dashboard development, this project includes a forecasting and predictive analytics component.
The forecasting portion explores hotel booking demand behavior, seasonal fluctuations, and reservation trends to support operational planning and demand prediction.

[Predictive Analytics & Forecasting](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/predictive-analytics.md)

---

## Dashboard Overview

### 1. Cancellation Overview Dashboard

#### Key Insights

| Insight | Business Impact |
|---|---|
| Overall cancellation rate reached **27.51%** | Significant operational and revenue risk |
| Booking demand peaked during summer months | Seasonal staffing and pricing opportunities |
| Online and Offline TA/TO segments showed elevated cancellations | Third-party channels contribute higher uncertainty |
| Longer booking lead times correlated with higher cancellation rates | Early reservations carry greater cancellation risk |
| Tuesday and Wednesday showed the highest negative cancellation variance | Midweek booking behavior may require closer monitoring |

#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Introduce flexible pricing tied to cancellation risk | Improve occupancy forecasting |
| Incentivize direct bookings | Reduce OTA cancellation exposure |
| Implement dynamic cancellation policies for long lead-time bookings | Reduce lost room inventory |
| Improve predictive monitoring during peak booking seasons | Optimize staffing and room availability |



---

## 2. ADR Performance Dashboard

#### Key Insights

| Insight | Business Impact |
|---|---|
| Average ADR reached approximately **$106.48** | Strong pricing performance overall |
| ADR peaked during summer months | Seasonal demand drives pricing opportunities |
| Resort hotels consistently achieved higher ADR values | Resort customers demonstrate higher spending behavior |
| No-deposit reservations generated the highest ADR values | Flexible booking customers may provide higher revenue potential |
| ADR distribution varied widely across market segments | Customer segmentation strongly influences pricing performance |

#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Increase premium pricing during peak seasonal periods | Maximize high-demand revenue |
| Develop loyalty incentives for high-value customer groups | Improve repeat customer retention |
| Expand upsell opportunities in resort properties | Increase guest spending per stay |
| Adjust pricing dynamically by booking segment and seasonality | Improve ADR optimization |

---

## 3. Booking Behavior & Customer Insights Dashboard

#### Key Insights

| Insight | Business Impact |
|---|---|
| Online bookings generated the largest booking volume | Digital channels dominate customer acquisition |
| Couples represented the largest booking group size | Marketing strategies should prioritize couple travel packages |
| Short and medium stay durations produced stronger ADR values | Shorter stays may provide higher room turnover efficiency |
| Very long lead-time bookings showed weaker ADR performance | Long-term reservations may reduce pricing flexibility |
| ADR distribution displayed significant outliers across booking channels | High-spending customer segments exist within specific channels |

#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Prioritize digital marketing campaigns | Improve booking conversion rates |
| Create targeted packages for couples and family travelers | Increase customer engagement |
| Optimize stay-length pricing strategies | Improve room profitability |
| Monitor outlier spending behavior for premium service opportunities | Increase luxury revenue streams |

---

## Visualization Techniques Used

| Visualization | Purpose |
|---|---|
| KPI Cards | Executive summary metrics |
| Dual-Axis Trend Charts | Booking demand vs cancellation trends |
| Sankey Diagram | Customer segment cancellation flow |
| Box & Whisker Plot | ADR distribution analysis |
| Bubble Chart | Booking volume vs ADR relationship |
| Histograms | ADR distribution comparison |
| Bar Charts | Segment and seasonal comparisons |
| Dot Plots | Weekly ADR analysis |

---

## Tools & Technologies

| Tool | Purpose |
|---|---|
| Tableau | Dashboard development and visualization |
| Excel / CSV | Data preparation |
| SQL | Data exploration and analysis |
| Python (optional) | Exploratory analysis and preprocessing |

---

## Conclusion

The Avalon Hotels Booking Analytics project demonstrates how hospitality organizations can leverage data visualization and operational analytics to improve booking management, pricing strategies, and customer segmentation decisions.

The analysis identified several high-impact operational patterns, including elevated cancellation behavior among OTA channels, strong seasonal ADR fluctuations, and substantial differences in customer value across booking types and hotel categories.

These findings highlight opportunities to improve occupancy forecasting, reduce cancellation-related revenue loss, and optimize dynamic pricing strategies.

By combining KPI dashboards, customer behavior analysis, and interactive filtering capabilities, the project provides executives and revenue management teams with actionable insights to support data-driven decision-making in the hospitality industry.

---

# Future Enhancements

| Enhancement | Potential Value |
|---|---|
| Predictive cancellation modeling | Forecast high-risk reservations |
| Revenue forecasting integration | Improve financial planning |
| Customer lifetime value analysis | Identify high-value guests |
| Real-time booking monitoring | Enhance operational responsiveness |
| Geographic demand analysis | Support regional marketing strategies |

---

# Project Links

| Resource | Link |
|---|---|
| GitHub Repository | Insert GitHub Link Here |
| Tableau Public Dashboard | Insert Tableau Link Here |

---

# Dashboard Screenshots

## Cancellation Analytics Dashboard

![Cancellation Dashboard](assets/cancellation_dashboard.png)

---

## ADR Performance Dashboard

![ADR Dashboard](assets/adr_dashboard.png)

---

## Booking Behavior Dashboard

![Booking Behavior Dashboard](assets/booking_behavior_dashboard.png)
