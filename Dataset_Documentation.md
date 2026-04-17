# 📚 Customer Churn Analysis Dataset Documentation

---

## 🧠 Overview

This dataset represents user-level behavioral and subscription activity data used to analyze **customer churn patterns, retention drivers, and engagement behavior**.

It is designed to support **business intelligence dashboards and predictive churn analysis** across product, user, and platform dimensions.

---

## 🎯 Purpose

* Identify key drivers of customer churn
* Analyze user behavior across devices and networks
* Evaluate subscription plan effectiveness
* Measure impact of technical performance on retention
* Understand demographic and genre-based engagement patterns

---

## 📊 Key Business Metrics

* **Total Users:** 4,600
* **Active Users:** 3,188
* **Churned Users:** 1,412
* **Churn Rate:** 30.70%

---

## 📦 Data Dictionary (Unified)

| Column Name                | Data Type | Description                                                       |
| -------------------------- | --------- | ----------------------------------------------------------------- |
| user_id                    | String    | Unique identifier for each user                                   |
| gender                     | String    | Gender of the user                                                |
| age_group                  | String    | Age segmentation                                                  |
| top_genre                  | String    | Most engaged content genre for the user                           |
| subscription_plan          | String    | Current active plan                                               |
| payment_method             | String    | Method used for subscription payment                              |
| auto_renewal_enabled       | Boolean   | Indicates whether auto-renewal is enabled                         |
| previous_subscription_plan | String    | User’s previous subscription tier                                 |
| device_type                | String    | Platform used                                                     |
| network_type               | String    | Connectivity type                                                 |
| buffering_time_avg         | Float     | Average buffering delay experienced by user                       |
| is_churned                 | Boolean   | Target variable indicating churn status                           |

---

## 🔗 Relationship Logic (Business Perspective)

* Each row represents a **unique user profile and behavior snapshot**
* Subscription and payment attributes define **monetization behavior**
* Device + network data reflects **technical experience quality**
* Buffering time acts as a **performance-to-churn risk indicator**
* Genre preference connects **content engagement with retention**
* `is_churned` serves as the **target outcome variable for churn modeling**

---

## 📐 Business Rules

* Each record represents one unique user
* No duplicate `user_id` entries are allowed
* `is_churned` is derived from user inactivity or subscription drop-off
* Buffering time is aggregated as an average per user session history
* Subscription changes are tracked via previous vs current plan comparison

---

## 📊 Analytical Scope

This dataset enables analysis across:

* Customer churn prediction and segmentation
* Device-wise retention performance
* Subscription plan effectiveness
* Impact of buffering/latency on churn behavior
* Payment method and auto-renewal influence on retention
* Demographic and content preference analysis

---

## ⚠️ Data Considerations

* High buffering time strongly correlates with churn risk
* Mobile users (Android/iOS) may show higher churn volatility
* Non-auto-renew users are at higher risk of churn
* Subscription transitions may indicate downgrade/upgrade behavior patterns
* Certain age groups may show uneven engagement distribution

---

## 🚀 Usage Context

This dataset is designed for:

* Power BI / Tableau dashboards
* Churn prediction models (ML use cases)
* Customer segmentation analysis
* Product experience optimization
* Business retention strategy design

---

## 🧠 Closing Insight

This dataset goes beyond user tracking — it functions as a **behavioral intelligence system** that connects product experience, technical performance, and monetization strategy to explain customer churn at scale.
