<img width="800" 
height="450" alt="Avalon Hotels Analytics Suite" 
src="https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/assets/avalon-hotels-analytics-suites-logo.png"/>

# Avalon Hotels Booking Analytics Suite

## Executive Summary

The Avalon Hotels Booking Analytics project analyzes hotel reservation patterns, cancellation behavior, and Average Daily Rate (ADR) performance to uncover operational risks and revenue optimization opportunities across resort and city hotels.

The analysis reveals that cancellation behavior varies significantly across customer segments, booking lead times, and booking channels. The overall cancellation rate reached **27.51%**, indicating that more than one in four bookings were canceled prior to arrival.

High-risk segments such as Online Travel Agencies (OTAs) and long lead-time reservations contributed disproportionately to cancellations, while direct bookings and shorter lead times demonstrated stronger booking stability.

Additional analysis of ADR trends identified seasonal pricing fluctuations, differences between hotel types, and varying customer value across booking behaviors. Resort hotels generally achieved higher ADR values than city hotels, while booking channels and deposit policies strongly influenced pricing performance.

The dashboards were designed to support hotel executives, revenue managers, and operational teams with interactive KPI monitoring, booking behavior analysis, and data-driven pricing and cancellation reduction strategies.

---

# Project Objectives

| Objective | Business Goal |
|---|---|
| Analyze hotel booking trends | Identify seasonal booking demand patterns |
| Evaluate cancellation behavior | Reduce revenue loss from booking cancellations |
| Investigate ADR performance | Improve pricing and occupancy strategies |
| Compare hotel types and customer segments | Understand high-value and high-risk customer groups |
| Develop executive dashboards | Support operational and strategic decision-making |

---

# Key Metrics Measured

| Metric | Description |
|---|---|
| Cancellation Rate | Percentage of bookings canceled before arrival |
| Total Bookings | Total reservation volume |
| Total Cancellations | Number of canceled reservations |
| ADR (Average Daily Rate) | Average revenue earned per occupied room |
| Booking Lead Time | Time between reservation and arrival |
| Market Segment Performance | Booking and cancellation trends across customer groups |
| Hotel Type Performance | Comparison between City and Resort hotels |
| Stay Length | ADR and booking behavior by duration of stay |

---

# Dataset Overview

| Attribute | Details |
|---|---|
| Dataset Type | Hotel Booking Demand Dataset |
| Hotel Types | City Hotel & Resort Hotel |
| Time Period | July 2015 to Aug 2017 |
| Records | Approximately ___ hotel bookings |
| Features | Reservation details, customer type, ADR, lead time, cancellations, deposit type, booking channel, stay duration |
| Data Source | Kaggle / Public Hospitality Dataset |

---

# Data Dictionary

| Field | Description |
|---|---|
| is_canceled | Indicates whether the booking was canceled |
| adr | Average Daily Rate charged for the booking |
| hotel | Hotel category (City or Resort) |
| market_segment | Booking acquisition segment |
| lead_time | Days between booking and arrival |
| customer_type | Type of customer reservation |
| arrival_date_month | Arrival month |
| arrival_date_week_number | Week of arrival |
| stays_in_week_nights | Number of weekday nights |
| stays_in_weekend_nights | Number of weekend nights |
| deposit_type | Deposit policy selected |
| adults / children / babies | Number of guests |
| reservation_status | Final reservation outcome |

---

## Predictive Analytics & Forecasting

In addition to Tableau dashboard development, this project includes a forecasting and predictive analytics component.
The forecasting portion explores hotel booking demand behavior, seasonal fluctuations, and reservation trends to support operational planning and demand prediction.

➡️ [Predictive Analytics & Forecasting](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/predictive-analytics.md)

---

# Dashboard Overview

# 1. Cancellation Overview Dashboard

## Key Insights

| Insight | Business Impact |
|---|---|
| Overall cancellation rate reached **27.51%** | Significant operational and revenue risk |
| Booking demand peaked during summer months | Seasonal staffing and pricing opportunities |
| Online and Offline TA/TO segments showed elevated cancellations | Third-party channels contribute higher uncertainty |
| Longer booking lead times correlated with higher cancellation rates | Early reservations carry greater cancellation risk |
| Tuesday and Wednesday showed the highest negative cancellation variance | Midweek booking behavior may require closer monitoring |

## Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Introduce flexible pricing tied to cancellation risk | Improve occupancy forecasting |
| Incentivize direct bookings | Reduce OTA cancellation exposure |
| Implement dynamic cancellation policies for long lead-time bookings | Reduce lost room inventory |
| Improve predictive monitoring during peak booking seasons | Optimize staffing and room availability |



---

# 2. ADR Performance Dashboard

## Key Insights

| Insight | Business Impact |
|---|---|
| Average ADR reached approximately **$106.48** | Strong pricing performance overall |
| ADR peaked during summer months | Seasonal demand drives pricing opportunities |
| Resort hotels consistently achieved higher ADR values | Resort customers demonstrate higher spending behavior |
| No-deposit reservations generated the highest ADR values | Flexible booking customers may provide higher revenue potential |
| ADR distribution varied widely across market segments | Customer segmentation strongly influences pricing performance |

## Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Increase premium pricing during peak seasonal periods | Maximize high-demand revenue |
| Develop loyalty incentives for high-value customer groups | Improve repeat customer retention |
| Expand upsell opportunities in resort properties | Increase guest spending per stay |
| Adjust pricing dynamically by booking segment and seasonality | Improve ADR optimization |

---

# 3. Booking Behavior & Customer Insights Dashboard

## Key Insights

| Insight | Business Impact |
|---|---|
| Online bookings generated the largest booking volume | Digital channels dominate customer acquisition |
| Couples represented the largest booking group size | Marketing strategies should prioritize couple travel packages |
| Short and medium stay durations produced stronger ADR values | Shorter stays may provide higher room turnover efficiency |
| Very long lead-time bookings showed weaker ADR performance | Long-term reservations may reduce pricing flexibility |
| ADR distribution displayed significant outliers across booking channels | High-spending customer segments exist within specific channels |

## Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Prioritize digital marketing campaigns | Improve booking conversion rates |
| Create targeted packages for couples and family travelers | Increase customer engagement |
| Optimize stay-length pricing strategies | Improve room profitability |
| Monitor outlier spending behavior for premium service opportunities | Increase luxury revenue streams |

---

# Visualization Techniques Used

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

# Tools & Technologies

| Tool | Purpose |
|---|---|
| Tableau | Dashboard development and visualization |
| Excel / CSV | Data preparation |
| SQL | Data exploration and analysis |
| Python (optional) | Exploratory analysis and preprocessing |

---

# Conclusion

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
