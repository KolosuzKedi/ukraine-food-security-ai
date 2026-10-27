# ukraine-food-security-ai
This repository contains an AI-based machine learning solution that forecasts food price fluctuations and detects abnormal price spikes in conflict and crisis-affected regions, focusing on Ukraine. The objective is to provide an early warning mechanism*for humanitarian organizations and public institutions to support targeted interventions.
## 📌 Project Overview & SDG Alignment

* **Sustainable Development Goal:** **SDG 2 — Zero Hunger** / *Target 2.1: Universal access to safe, nutritious, and sufficient food*
* **Problem Statement:** During periods of conflict and crisis, severe supply chain disruptions, regional market collapse, and soaring food inflation significantly threaten household food security.
* **Solution:** A predictive machine learning pipeline using World Food Programme (WFP) data to accurately model regional and commodity-level price dynamics and flag market anomalies.

---

## 📊 Dataset Summary

* **Data Source:** World Food Programme (WFP) — Ukraine Food Prices Dataset
* **Observations:** 5,136 records (after data cleaning and missing value treatment)
* **Key Features:**
  * **Temporal:** `date`, `year`, `month`
  * **Geographic:** `county`, `subcounty`, `market`, `latitude`, `longitude`
  * **Commodity Details:** `category`, `commodity`, `unit`
  * **Target Variable:** `price_usd`

---

## 🤖 Model & Performance

A **Random Forest Regressor** model was selected for its ability to capture non-linear relationships and complex spatial-commodity interactions without requiring strict distributional assumptions.

### Baseline Evaluation Metrics:
* **MAE (Mean Absolute Error):** `$0.0423 USD`
* **RMSE (Root Mean Squared Error):** `$0.0839 USD`

