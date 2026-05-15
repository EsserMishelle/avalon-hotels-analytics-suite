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

The Avalon Hotels Analytics Suite contains reservation information for both resort hotels and city hotels between July 2015 and August 2017. The Hotel Booking Demand Dataset includes hotel reservation records and operational features related to customer segmentation, Average Daily Rate (ADR), booking lead time, cancellation behavior, booking channels, deposit policies, and stay duration.

## Exploratory Data Analysis

Exploratory analysis was conducted to better understand reservation behavior, identify data quality issues, and evaluate patterns associated with hotel booking cancellations and pricing performance.

The analysis revealed:

- **119,390 reservation records** across **32 variables**
- Missing values across several operational fields, including children (4), country (452), agent (12,193), and company (82,137)
- Approximately **31,994 duplicate reservation entries**
- Significant variation in booking behavior across hotel types, customer segments, pricing patterns, and cancellation activity

### Data Cleaning & Preparation

- Removed duplicate reservation records
- Handled missing and null values
- Performed feature engineering and data transformation
- Standardized selected categorical variables
- Prepared data for exploratory analysis and predictive modeling workflows

After preprocessing and transformation, the final analytical dataset contained approximately **87,213 records** across **32 columns**.

The original dataset, cleaned dataset, and complete data dictionary containing detailed field definitions and variable descriptions are attached below.

[Original Dataset](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/hotels.csv)  
[Cleaned Dataset](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/clean_hotels.csv)  
[Avalon Hotels Data Dictionary](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/assets/avalon_hotels_data_dictionary.xlsx)

---

## Tableau Visualization

The visual analysis and dashboard development were conducted in Tableau to support operational monitoring, pricing analysis, customer segmentation, and cancellation trend evaluation.

[Avalon Hotels Analytics Suite Tableau Workbook](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/avalon-hotels-analytics-suites.twbx)

---

## Predictive Analytics & Forecasting

In addition to Tableau dashboard development, this project includes a predictive analytics and forecasting component focused on hotel booking demand behavior, seasonal fluctuations, and reservation cancellation prediction.

The forecasting analysis supports operational planning, occupancy forecasting, and predictive modeling workflows within the hospitality industry.

[Predictive Analytics & Forecasting](https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/predictive-analytics.md)


---

## Cancellation Analysis

### 1. Cancellation Overview 

<img width="1286" height="576" alt="image" src="https://github.com/user-attachments/assets/c4924408-6dc9-4889-84f8-a4534a066f7e" />
<img width="1285" height="416" alt="image" src="https://github.com/user-attachments/assets/54eb41aa-2e9e-490c-a62c-2251d2fdc095" />

#### Key Findings 

- Overall cancellation rate reached **27.51%**, or 24k of 87.2k total bookings.
- The highest cancellation rate was observed among **Transient City Hotel customers**, while **Group Resort Hotel bookings** demonstrated the lowest cancellation behavior at approximately **6%**.
- Cancellation behavior varied by weekday, with **Friday showing the highest cancellation activity** and **Tuesday demonstrating the lowest cancellation rate**.
- Booking lead time strongly influenced cancellation behavior. Long lead-time reservations for **City Hotels reached approximately 52% cancellation**, while comparable Resort Hotel bookings remained significantly lower at approximately **6%**.
- Seasonal booking trends revealed that **August experienced the highest booking demand and cancellation activity**, reaching approximately **11K bookings with a 32% cancellation rate**.
- **November recorded the lowest booking volume at approximately 5K reservations** and maintained one of the lowest cancellation rates at approximately **21%**.
- Market segment analysis showed that **Corporate** and **Complementary** bookings maintained relatively low cancellation rates near **12%**, while **Online Travel Agency (OTA)** bookings reached approximately **35% cancellation**, representing the highest-risk booking segment.

#### Business Insights

- Overall cancellation is more than 1 of 4 bookings, which could cause significant operational and revenue risk.
- Booking demand peaked during summer months which provides seasonal staffing and pricing opportunities
- Third-party or Online Travel Agency (OTA) channels generate substantial booking volume but also contribute disproportionately to operational uncertainty and potential revenue loss due to elevated cancellation behavior.
- Long lead-time reservations create increased forecasting risk, particularly within City Hotels where cancellation exposure is significantly higher.
- Resort Hotel group bookings appear more stable and predictable, suggesting stronger customer commitment and lower booking volatility.
- Seasonal demand spikes during August may require enhanced staffing, inventory planning, and cancellation management strategies to minimize operational disruption.


#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Introduce flexible pricing tied to cancellation risk | Improve occupancy forecasting |
| Incentivize direct bookings | Reduce OTA cancellation exposure |
| Implement dynamic cancellation policies for long lead-time bookings | Reduce lost room inventory |
| Improve predictive monitoring during peak booking seasons | Optimize staffing and room availability |

<br>

---
### 2. Cancellation Risk Drivers

<img width="1291" height="662" alt="image" src="https://github.com/user-attachments/assets/e4ebfb7a-c229-4df8-8cf8-8893af204905" />
<img width="1282" height="331" alt="image" src="https://github.com/user-attachments/assets/24aea432-cbe3-413b-9a89-b684933ecad1" />

#### Key Findings

- Third-party or Online Travel Agency (OTA) bookings represented the highest-risk market segment, reaching approximately **35% cancellation** while also generating the largest booking volume.
- Group bookings maintained relatively lower cancellation pattern despite moderate booking volume, indicating stronger reservation stability compared to OTA channels.
- Long and very long booking lead times demonstrated significantly higher cancellation rates, particularly among non-refundable reservations.
- Very long lead-time reservations combined with Non-Refundable deposit policies demonstrated the highest observed cancellation exposure, reaching nearly **100% cancellation** rate within that booking category.
- Couples represented the largest booking group composition, significantly exceeding solo travelers, families, and large groups in reservation volume.
- Customers with higher numbers of special requests exhibited lower cancellation behavior, suggesting stronger booking commitment and customer intent.
- Guests with previous cancellation history showed elevated future cancellation risk, with cancellation rates peaking near **80%** among customers with one prior cancellation.


#### Business Insights

- OTA channels contribute substantial booking demand but simultaneously create elevated operational uncertainty and forecasting risk.
- Long lead-time reservations appear less reliable and may require additional monitoring, deposit requirements, or dynamic cancellation policies.
- Customers demonstrating stronger engagement behaviors, such as applying for special requests, appear more committed to completing reservations.
- Historical cancellation behavior serves as a strong indicator of future cancellation risk, suggesting opportunities for predictive customer risk scoring.
- Couples and family travelers represent important customer segments that may support targeted loyalty, retention, and bundled travel strategies.


#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Implement stricter cancellation or deposit policies for high-risk OTA reservations | Maintain exposure to third-party channel while reducing cancellation-related revenue loss |
| Apply predictive risk monitoring for guests with prior cancellation history | Improve occupancy forecasting accuracy |
| Encourage direct booking incentives and loyalty programs | Increase reservation stability and reduce OTA dependence |
| Introduce targeted retention offers for high-risk long lead-time reservations | Improve booking conversion and occupancy retention |
| Prioritize customer engagement features such as special request personalization | Strengthen customer commitment and reduce cancellations |
| Develop tailored marketing packages for couples and family visitors | Improve customer retention and revenue opportunities |

<br>

---
## Average Daily Rate (ADR) Analysis

### 1. ADR Overview

<img width="1302" height="1000" alt="image" src="https://github.com/user-attachments/assets/147713e5-198e-4603-b3c5-9ee7823112f8" />

#### Key Findings

- Avalon Hotels generated approximately **87.2k** total bookings and **$23.0M in total revenue** while maintaining an average ADR of approximately **$106.48**.
- ADR performance demonstrated strong seasonality, with pricing peaking during the summer months, particularly in **July and August**, where ADR exceeded approximately **$140–$150**.
- ADR trends declined noticeably during the late fall and winter months reaching approximately **$70-$80**, indicating lower seasonal demand and reduced pricing power.
- Customers with **No Deposit reservations** generated the highest ADR values, while refundable bookings maintained lower average pricing performance.
- Transient traverlers produced the highest ADR among customer types, outperforming contract, group, and transient-party bookings.
- Friday and Saturday generated the strongest ADR performance across weekdays, suggesting increased weekend demand and higher customer willingness to pay.
- ADR distribution analysis revealed significant variability across market segments, with **Online Travel Agencies (OTA)** and **Direct bookings** containing the widest pricing ranges and highest-value reservation outliers.
- Market segments such as Complementary and Corporate bookings maintained lower ADR distributions and narrower pricing variability compared to OTA and Direct channels.


#### Business Insights

- Seasonal demand significantly influences hotel pricing performance, with summer travel periods creating stronger revenue optimization opportunities.
- Lower ADR performance during November may be associated with reduced seasonal travel demand during the late fall period.
- Weekend travel demand appears substantially stronger than midweek demand, supporting dynamic weekend pricing strategies.
- Transient travelers and OTA channels represent high-revenue customer segments but may also require more active pricing and careful inventory management.
- Large ADR variability within OTA and Direct booking channels suggests opportunities for premium segmentation, upselling, and targeted pricing optimization.
- Lower ADR values among contract and group bookings may reflect negotiated pricing structures or long-term occupancy agreements that prioritize occupancy stability over premium pricing.


#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Increase dynamic pricing during peak summer periods | Maximize seasonal revenue opportunities |
| Target promotions during low-demand seasons | Increase revenue and occupancy during slower travel periods |
| Apply premium weekend pricing strategies | Improve ADR performance during high-demand travel periods |
| Expand upsell and premium room offerings within OTA and Direct channels | Increase high-value booking revenue |
| Increase promotion to transient travelers | Reduce last-minute occupancy and increase revenue |
| Develop targeted retention campaigns for transient travelers | Improve customer lifetime value and repeat bookings |
| Optimize pricing strategies during low-demand months | Improve occupancy stability and revenue consistency |
| Segment pricing strategies by customer type and booking channel | Improve revenue optimization across customer groups |
| Monitor ADR outliers and premium booking behavior | Identify luxury customer opportunities and pricing trends |


---

### 2. ADR Performance Drivers
<img width="1300" height="1000" alt="image" src="https://github.com/user-attachments/assets/27bfd40d-a80d-405f-a5cb-541b69810f7c" />

#### Key Findings

- Avalon Hotels generated approximately **87.2K total bookings** and **$23.0M in total revenue**, while maintaining an average ADR of approximately **$106.48**.
- Online Travel Agency (OTA) bookings generated the highest booking volume while also maintaining one of the highest ADR values among booking segments.
- Direct bookings achieved premium ADR performance despite lower booking volume, positioning them as high-value niche customer segments.
- Corporate and complementary bookings maintained lower ADR values compared to OTA and Direct channels.
- ADR performance was strongest for stays between **6–10 nights** for approximately **$113 ADR**, while very long stays demonstrated lower average pricing performance.
- Short and medium booking lead times produced the highest ADR values **($116 and $112)**, while very long lead-time reservations generated lower ADR performance.
- City Hotels demonstrated wider ADR variability and a broader pricing distribution compared to Resort Hotels.
- Couples represented the largest guest composition segment, significantly exceeding solo travelers and family bookings in reservation volume.
- Non-deposit reservations generated the highest ADR values, while refundable bookings maintained the lowest average pricing performance.

#### Business Insights

- OTA and Direct booking channels represent the strongest revenue-driving customer segments due to their combination of higher ADR performance and substantial booking activity.
- Premium ADR performance among Direct bookings suggests opportunities to expand loyalty, membership, and direct marketing initiatives.
- Lower ADR among long lead-time reservations may indicate early-booking discounts or lower pricing flexibility over extended planning periods.
- Wider ADR variability within City Hotels suggests greater exposure to fluctuating pricing strategies, customer demand shifts, and dynamic market conditions.
- Guest composition trends indicate that couples and family travelers represent important customer segments for pricing optimization and promotional targeting.

#### Strategic Recommendations

| Recommendation | Expected Outcome |
|---|---|
| Expand direct booking incentives and loyalty programs | Increase high-value direct reservation volume and reduce OTA dependency |
| Apply dynamic pricing strategies during high-demand booking periods | Improve ADR optimization and pricing flexibility |
| Increase premium upsell opportunities within OTA channels | Maximize revenue potential from high-volume booking segments |
| Develop targeted promotions for long-stay reservations | Improve ADR performance across extended bookings |
| Monitor pricing variability across City Hotels | Improve pricing consistency and operational forecasting |
| Create bundled packages for couples and family travelers | Increase customer retention and booking value |
| Optimize seasonal pricing strategies during lower-demand periods | Improve occupancy and stabilize ADR performance |

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

