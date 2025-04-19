# SC1015 Mini Project
# 🏨 Hotel Reservation Cancellation Prediction

## 📌 Project Overview
This project investigates patterns behind hotel reservation cancellations and builds a machine learning model to **predict cancellations in advance** using booking-time features. The goal is to help hotels shift from reactive to proactive management of cancellations, improving both operational efficiency and revenue retention.

---

## 🎯 Objectives
1. Identify which booking features are most strongly associated with cancellations.
2. Develop and evaluate predictive models to accurately classify high-risk bookings.

---

## 📊 Dataset
- **Source**: `train__dataset.csv`
- **Rows**: 18,137 hotel bookings
- **Target**: `booking_status` (0 = Not Cancelled, 1 = Cancelled)
- **Key features used**:
  - `lead_time`
  - `avg_price_per_room`
  - `no_of_special_requests`
  - `room_type_reserved`
  - `arrival_month`, `customer_type`, `market_segment_type`

---

## 🧪 Data Analysis & Key Insights
- **Longer lead times** → Higher cancellation risk (ρ = 0.41)
- **More special requests** → Lower risk, indicating commitment (ρ = -0.25)
- **Price extremes** → More cancellations, due to sensitivity or regret
- **Seasonality** → Certain months have noticeably higher cancellation rates
- **Repeated guests** → More reliable, fewer cancellations

Statistical tests used:
- **Spearman Correlation** (for ranked variables)
- **Chi-Square & Cramér’s V** (for categorical associations)

---

## 🤖 Models Used
We evaluated five machine learning models:

| Model                | Accuracy | Precision (Cancelled) | Recall (Cancelled) |
|----------------------|----------|------------------------|---------------------|
| Decision Tree        | 79%      | 73%                    | 60%                 |
| Linear Regression    | 79%      | 76%                    | 51%                 |
| Random Forest        | 81%      | 82%                    | 54%                 |
| Support Vector Machine (SVM) | 78% | 63%               | 76%                 |
| **Gradient Boosting**| **82%**  | **80%**                | **61%**             |

✅ **Gradient Boosting** was the best-performing model overall.

---

## 🔍 Top Predictive Features
1. **Lead Time**: Longer time before check-in → more cancellations  
2. **No. of Special Requests**: More requests → lower cancellations  
3. **Average Price Per Room**: Price-sensitive guests more likely to cancel

---

## 🧠 Key Takeaways
- Cancellations follow **predictable patterns** based on booking behavior.
- **Early prediction** enables smarter overbooking, targeted guest outreach, and better staffing.
- Models like Gradient Boosting offer **reliable accuracy with interpretable features**.

---

## 📂 Files
- `main.ipynb`: Full notebook with EDA, visualizations, and model training
- `train__dataset.csv`: Dataset used for training and evaluation
- `README.md`: Project summary and instructions

---

## ✨ Future Work
- Incorporate time-series forecasting for cancellation trends
- Add text analysis (e.g. guest feedback)
- Test deployment in a real-time hotel reservation system

---

## 🧑‍💻 Author
Swaminathan Navitraa (U2321255K)  
Shruti Kannan 

---


