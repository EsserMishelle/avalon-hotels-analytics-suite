<img width="800" height="450" alt="Avalon Hotels Analytics Suite" src="https://github.com/EsserMishelle/avalon-hotels-analytics-suite/blob/main/assets/avalon-hotesl-predictive-modeling-logo.png" />


# Avalon Hotels Predictive Analytics

## Overview

Avalon Hotels Predictive Analytics explores hotel booking cancellation behavior using exploratory data analysis (EDA), forecasting techniques, and machine learning models.

Using reservation data from resort and city hotels, the project analyzes patterns related to booking lead time, customer segmentation, booking channels, and seasonal demand to identify factors associated with hotel reservation cancellations.

The analysis focuses on predictive modeling techniques that support occupancy planning, revenue management, and operational forecasting within the hospitality industry.

---

## Business Problem

Hotel cancellations create significant operational and revenue challenges for hospitality organizations. Unexpected cancellations can negatively impact occupancy forecasting, staffing allocation, pricing strategies, and overall revenue performance.

This project applies predictive analytics to identify cancellation risk patterns and evaluate machine learning models capable of supporting more proactive operational decision-making.

---

## Project Objectives

The primary objectives of this project are to:
- analyze hotel booking and cancellation behavior,
- identify operational patterns associated with reservation cancellations,
- evaluate predictive machine learning models.

## Dataset

<img width="1022" height="188" alt="DataFrame summary" src="https://github.com/user-attachments/assets/0c6fa01b-7497-432a-965b-2add5ee65410" />

<img width="1307" height="183" alt="Cleaned dataset summary" src="https://github.com/user-attachments/assets/00ea089d-a4e4-4e30-8314-67e149a9418a" />

This project uses the **Hotel Booking Demand Dataset** from **Kaggle**, which contains reservation information for both resort hotels and city hotels.

## Exploratory Data Analysis

Exploratory analysis was conducted to better understand reservation behavior, identify data quality issues, and evaluate patterns associated with hotel booking cancellations.

The analysis revealed:

-  **119,390 reservation records** across **32 variables**, 
- missing values across several operational fields: children (4), country (452), agent (12,193) and company (82,137). 
- approximately **31,994 duplicate reservation entries**,
- and notable variation in booking behavior across segments and hotel types, covering booking details, customer information, stay duration, pricing metrics, booking channels, and cancellation indicators.

---

### Data Cleaning and Preparation

- Removed duplicate reservation records
- Handled missing and null values
- Performed feature engineering and data transformation
- Standardized selected categorical variables
- Prepared data for exploratory analysis and predictive modeling workflows

After data cleaning, duplicate removal, and feature transformation, the final analytical dataset contained **87,213 records** and **32 columns**.

---

## Key Variables Used in the Analysis

The analysis focuses on operational and customer-related variables most relevant to hotel booking behavior and cancellation prediction.

| Variable | Description |
|---|---|
| hotel | Hotel category (City Hotel or Resort Hotel) |
| lead_time | Number of days between booking and arrival |
| arrival_date_year | Arrival year |
| arrival_date_month | Arrival month |
| stays_in_weekend_nights | Number of weekend nights booked |
| stays_in_week_nights | Number of weekday nights booked |
| adults / children / babies | Guest composition |
| market_segment | Booking acquisition segment |
| is_canceled | Reservation cancellation indicator |
| adr | Average Daily Rate (room price per night) |
| customer_type | Customer reservation category |

These variables were selected because they support analysis of:
- cancellation behavior,
- customer segmentation,
- booking demand patterns,
- occupancy trends,
- and pricing performance.

---

## EDA Charts 

**Cancellation Distribution and Cancellation By Hotel Type**

<img width="533" height="353" alt="image" src="https://github.com/user-attachments/assets/786cb9bd-9afd-4fbc-8b94-637f6ed4e468" />

Most bookings are completed, but cancellation rates differ by hotel type, with city hotels experiencing more cancellations than resort hotels.

**Lead Time vs. Cancellation**

<img width="395" height="305" alt="image" src="https://github.com/user-attachments/assets/c605c16d-182a-4c73-bf63-6e4e5ab7198f" />

The median lead time for cancled booking is around 80 days. The canceled box is also wider/longer, which means there's more variability in lead time. The upper whisker is much higher for the cancel boxplot, indicating some bookings made very far in advance have been canceled. Cancelled bookings generally have longer lead times than non-cancelled bookings, suggesting that reservations made further in advance are more uncertain.

**Cancellation by Market Segment**

<img width="669" height="413" alt="image" src="https://github.com/user-attachments/assets/a4ef28fe-a8ed-4275-adb8-b888c107106c" />

Cancellation rates are highest for Groups and Online TA bookings and lowest for Corporate and Complementary bookings.

**Cancellation by market segment across channels**

<img width="505" height="342" alt="image" src="https://github.com/user-attachments/assets/b3fe4026-7c79-4c78-8fe6-602b679a782b" />

The heatmap illustrates cancellation rates across combinations of market segments and distribution channels. Higher cancellation rates are observed in indirect booking channels, particularly for Online Travel Agency (Online TA) segments through TA/TO channels. In contrast, direct bookings exhibit lower cancellation rates, indicating stronger customer commitment. 


These findings highlight the importance of booking channel and customer segment in predicting cancellation behavior.


**Cancellation by Weekdays**

<img width="580" height="382" alt="image" src="https://github.com/user-attachments/assets/eb8f6f92-8ca1-422d-85f1-0a6ec91ed22f" />

Cancellation rates increase toward the weekend, peaking on Friday (30.6%) and Saturday (30.1%). This pattern indicates that leisure travelers who are more likely to book weekend stays, show greater booking flexibility and higher cancellation behavior than weekday travelers.

**Average Monthly ADR and Cancellation Rate Chart**

<img width="857" height="437" alt="image" src="https://github.com/user-attachments/assets/6fa4393a-5b89-41d2-bd3f-a678e80b6d38" />

Higher ADR during peak months (June–August) coincides with elevated cancellation rates, highlighting a trade-off between revenue maximization and booking reliability. This suggests opportunities for strategies such as dynamic pricing, deposits, or overbooking to manage risk during high-demand periods.

**Cancellation by Deposit Type**

<img width="558" height="649" alt="image" src="https://github.com/user-attachments/assets/b5869b14-f90c-413b-9239-4d44b0fe49da" />

Most bookings are made without deposits. Non-refundable deposits show the highest cancellation rate, while refundable deposits have the lowest. However, refundable bookings account for only a small number of reservations, so **the percentage should be interpreted with caution.**

## Heatmap Chart

<img width="858" height="728" alt="image" src="https://github.com/user-attachments/assets/46cb378e-2010-45c4-b2dd-a96fe0506050" />


The heatmap shows several redundant variables. For example, total_nights is highly correlated with stays_in_week_nights (0.95) and stays_in_weekend_nights (0.78), while total_guests is strongly correlated with adults (0.74) and children (0.67). These relationships suggest overlapping information among features.

Most numerical features show weak correlations with booking cancellations. Lead time and average daily rate (ADR) show modest positive relationships with cancellations, while required parking spaces and special requests show negative relationships, suggesting stronger commitment among these bookings.

## Models
### Logistic Regression

A Logistic Regression model is used as the initial baseline classifier to predict booking cancellations. Since is_canceled is a binary outcome, Logistic Regression provides an interpretable and efficient starting point for evaluating how booking characteristics relate to cancellation behavior.

### Random Forest

Random Forest is a tree-based ensemble model to capture nonlinear relationships and interactions among booking features. Unlike Logistic Regression, which assumes a linear relationship between predictors and the outcome, Random Forest constructs multiple decision trees using bootstrapped samples of the data and aggregates their predictions. This approach can improve predictive performance and robustness, particularly when complex patterns exist in the dataset. The Random Forest model is evaluated alongside Logistic Regression to determine whether a more flexible, non-linear method improves cancellation prediction accuracy.

## Model Comparison
### Confusion Matrix

<img width="766" height="414" alt="image" src="https://github.com/user-attachments/assets/e2471e9b-fa79-4871-aeae-170a0812769f" />

## Model Evaulation
### Classification Report

<img width="430" height="551" alt="image" src="https://github.com/user-attachments/assets/a9770cd7-a509-4a9c-9a17-42d7618f6a55" />

The Logistic Regression classification report shows that when the model predicts that a booking will not be canceled, it is correct 90% of the time. It also correctly identifies 77% of cancellations, but its precision is lower (53%), meaning some bookings predicted as canceled are actually completed. This Logistic Regression is the first baseline model.

The Random Forest classification report shows that when the model predicts that a booking will not be canceled, it is slightly less correct 87% of the time. It also correctly identifying fewer cancellations at 63%, but its precision is higher (77%), meaning some bookings predicted as canceled are actually completed.

Random Forest achieves the highest overall accuracy (85% vs 75%) and precision when predicting cancellations. However, Logistic Regression has higher recall for canceled bookings, meaning it identifies a larger share of actual cancellations. This highlights the trade-off between minimizing false positives and capturing more true cancellations.

The F1-scores for both completed bookings and canceled bookings are higher for Random Forest (0.90 and 0.69) than for Logistic Regression (0.81 and 0.63). This indicates that Random Forest provides a better overall balance between precision and recall across both classes, resulting in stronger overall predictive performance.

### ROC Curves and AUC Scores

<img width="467" height="361" alt="image" src="https://github.com/user-attachments/assets/6c31d6c1-f4f0-455f-b5be-9af0df078e64" />

The ROC curve compares the classification performance of Logistic Regression and Random Forest across different probability thresholds. The Random Forest model achieves a higher AUC (0.91) than Logistic Regression (0.84), indicating a stronger ability to distinguish between canceled and non-canceled bookings.

The steeper and wider curve of the Random Forest model shows that it achieves a higher true positive rate for the same false positive rate across most thresholds. This suggests that Random Forest provides better overall predictive performance for the cancellation prediction task.

## Key Insights & Business Implications

### 1. Cancellation prediction can support hotel revenue management.

Within the Avalon Hotels Analytics Suite, predicting booking cancellations helps hotels anticipate occupancy loss and better manage operational planning. By identifying reservations with higher cancellation risk, hotels can adjust pricing strategies, promotional campaigns, staffing levels, and room inventory allocation to reduce potential revenue impact.

### 2. Model selection influences operational decision-making.

The comparison between Logistic Regression and Random Forest models demonstrates how different machine learning approaches can support different business priorities.

- Logistic Regression captures a larger share of actual cancellations, making it useful for identifying broader cancellation risk patterns.
- Random Forest delivers stronger overall predictive performance and more reliable cancellation classification, reducing unnecessary operational interventions caused by false positives.

### 3. Predictive trade-offs impact business strategy.

The analysis highlights the trade-off between recall and precision:

- If the operational goal is to identify as many potential cancellations as possible, Logistic Regression may be preferred.
- If the goal is to improve prediction reliability and reduce false alerts, Random Forest provides stronger performance.

This demonstrates how predictive model selection should align with specific hospitality business objectives.

### 4. Predictive analytics can improve operational efficiency.

Early identification of cancellation risk supports more proactive operational planning across:
- staffing allocation,
- occupancy management,
- marketing campaigns,
- and room availability forecasting.

These predictive insights can help hotels improve customer service responsiveness while optimizing revenue performance.

---

## Conclusion

As part of the Avalon Hotels Analytics Suite, this analysis evaluated Logistic Regression and Random Forest models for predicting hotel booking cancellations.

The results show that while Logistic Regression provides a strong baseline model and captures a larger share of actual cancellations, Random Forest achieves stronger overall predictive performance with higher accuracy and improved F1-scores across both booking classes.

The comparison demonstrates the value of predictive analytics and ensemble machine learning techniques when modeling complex hospitality booking behavior and cancellation trends.

Future enhancements to the Avalon Hotels Analytics Suite could include:
- forecasting hotel booking demand,
- predicting Average Daily Rate (ADR),
- expanding customer segmentation analysis,
- and integrating additional machine learning models to improve cancellation prediction performance.

➡️ Full Analysis: [Avalon Hotels Analytics Suite](avalon-hotels-analytics-suite.ipynb)
