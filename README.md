# 📊 New York Airbnb Listings EDA — 2024

## Overview
This project performs exploratory data analysis (EDA) on Airbnb listings in New York City for 2024. The analysis highlights trends in pricing, availability, room types, and host activity across boroughs. Visualizations are used to support insights and improve interpretability.

---

## Objectives
- Analyze distribution of room types and listing prices.
- Identify pricing trends across different neighborhoods.
- Examine host behavior and listing frequency.
- Detect price outliers and availability patterns.
- Provide actionable insights for hosts and guests.

---

## Dataset Summary
- **Rows:** 20,765  
- **Columns:** 22  
- **Key Features:**  
  - `id`, `name`, `host_name`  
  - `neighbourhood_group`, `latitude`, `longitude`  
  - `room_type`, `price`, `availability_365`  
  - `reviews_per_month`, `number_of_reviews`  

---

## Workflow

### 1. Data Cleaning
- Handled missing values in key columns (`price`, `beds`, `neighbourhood`).
- Converted `last_review` to datetime format.
- Capped extreme outlier prices above $1,000 for better visualization.

### 2. Exploratory Data Analysis
- **Room Types:** Bar plots to show frequency distribution.
- **Neighborhood Trends:** Grouped data by borough to compare pricing.
- **Price Distribution:** Histograms to understand price range.
- **Availability:** Heatmaps and pairplots to observe correlations.
- **Host Listings:** Boxplots to analyze multi-property hosts.
- **Review Activity:** Visualized relationship between reviews, price, and availability.

---

## Key Insights

- **Manhattan** has the highest average prices among all boroughs.
- **Entire home/apt** listings are the most common and the most expensive.
- Listings priced **$50–$300/night** make up the bulk of the market.
- Some hosts manage **10+ listings**, suggesting professional operations.
- Listings with **high availability** and **frequent reviews** are generally lower in price.

---

## Visualizations Used
- Bar charts  
- Histograms  
- Boxplots  
- Heatmaps  
- Pairplots

---

## Notes
- All analysis was done in Python using `pandas`, `matplotlib`, `seaborn`, and `numpy`.
- Outliers were addressed for clarity, but raw data is retained for reference.

---

## License
This project is open-source under the MIT License.

