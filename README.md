# 🏨 Hotel Reservation Cancellation Prediction

## 1. Problem Definition 
Our group defined the problem of predicting hotel reservation cancellations using a real-world dataset of 18,000+ bookings.  
Instead of merely describing booking trends, we **framed a predictive classification problem**:  
> *Can we predict whether a hotel reservation will be cancelled, using only features available at the time of booking?*

This business-focused problem allows for actionable strategies in overbooking, staffing, and revenue management.

---

## 2. Data Preparation & Cleaning
We used a dataset with 18 variables related to guest bookings. Key cleaning steps included:
- **Dropping missing values** (resulting in 18,137 clean records)
- **Encoding categorical variables** for model compatibility
- **Focusing only on booking-time features** to ensure real-world applicability
- Validating feature types and checking for outliers in numerical columns

These steps ensured the dataset was suitable for both statistical testing and machine learning.

---

## 3. Exploratory Data Analysis & Visualization 
We explored and visualized multiple patterns related to cancellations:
- **Lead time**: Longer lead times = higher cancellation rates  
- **Special requests**: More requests = fewer cancellations  
- **Average price**: Very high or very low prices → more cancellations  
- **Room type and seasonality** also showed noticeable trends

We used violin plots, histograms, count plots, and boxplots to surface these insights.  
Statistical tests (Spearman, Chi-Square, and Cramér’s V) were also applied to **quantify associations**.

---

## 4. Machine Learning Techniques 
We implemented and compared **five classification models**:
- Decision Tree  
- Linear Regression (adapted for binary outcomes)  
- Random Forest  
- Support Vector Machine  
- Gradient Boosting (best performance)

Best results from Gradient Boosting:
- **Accuracy:** 82%  
- **Precision (Cancelled class):** 80%  
- **Recall (Cancelled class):** 61%

We used ROC and Precision-Recall curves for performance evaluation. The top 3 predictive features were:
- `lead_time`
- `avg_price_per_room`
- `no_of_special_requests`

---

## 5. Data-Driven Insights & Recommendations 
Our analysis revealed actionable insights:
- **Longer lead times** → higher risk of cancellations  
- **Guests with special requests** are less likely to cancel  
- **Extreme pricing** (very high or low) correlates with more cancellations  
- **Repeated guests** are more reliable  

### Recommendations:
- Use cancellation scores to inform **smart overbooking strategies**  
- Send **reminders or promotions** to long-lead-time, no-request guests  
- Adjust staffing based on **seasonality and risk forecasts**

---

## 6. Final Presentation & Overall Quality 
We delivered a concise 10-minute presentation covering:
- Problem framing  
- Data exploration  
- Modeling approach  
- Evaluation metrics  
- Final insights & business recommendations

Presentation was supported by visuals, clean plots, and a structured narrative aligned to the business problem.

---

## 7. Learning & Going Beyond 
As a team, we went beyond course requirements by:
- **Applying three statistical tests** to strengthen EDA (Spearman, Chi-Square, Cramér’s V)
- Using **multiple evaluation metrics** beyond accuracy (precision, recall, AUC)  
- Building a practical pipeline with **real-world decision support value**
- Conducting a detailed feature importance comparison across models

This project gave us hands-on experience with **end-to-end data science**, from hypothesis-driven EDA to model deployment thinking.

---

## Files
- `main.ipynb`: Complete code and analysis notebook  
- `train__dataset.csv`: Cleaned dataset used  
- `README.md`: Project summary (this file)

---

## Team Members
- Swaminathan Navitraa (U2321255K)
- Shruti Kannan (U2323443H)

---



