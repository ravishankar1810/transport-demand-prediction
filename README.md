# 🚌 Mobiticket Transport Demand Prediction

## 📌 Project Description

### 📈 Business Context

Mobiticket is a ticketing platform that helps passengers book intercity bus tickets in Kenya. This project focuses on building a predictive model that estimates the **number of seats Mobiticket can expect to sell for each ride** on a specific date, time, and route.

There are **14 major routes**, all ending in **Nairobi**, originating from various towns in the northwest region of Kenya. These towns include:

- Awendo, Homa Bay, Kehancha, Kendu Bay, Keroka, Keumbu, Kijauri, Kisii, Mbita, Migori, Ndhiwa, Nyachenge, Oyugis, Rodi, Rongo, Sirare, and Sori

Each route follows a journey pattern with three stops in Nairobi:
1. **Kawangware** (first stop on the outskirts)
2. **Westlands**
3. **Afya Centre** (main bus terminal in the CBD)

Traffic conditions heavily impact arrival times and can influence a passenger’s booking decision, especially if arrival falls within peak traffic hours. Understanding **travel behavior and peak booking times** can help Mobiticket optimize fleet size, routing schedules, and dynamic pricing.

---

## 🧾 Data Description

The dataset includes historical ride and booking information with the following key features:

| Feature Name        | Description                                          |
|---------------------|------------------------------------------------------|
| `travel_date`       | Date of the ride                                     |
| `travel_time`       | Departure time of the ride                           |
| `route`             | Route name (origin town to Nairobi)                  |
| `booking_created`   | Timestamp when the booking was made                  |
| `Num_of_ticket`     | Number of tickets sold (target variable)             |
| `day_of_week`       | Day name extracted from `travel_date`                |
| `month`             | Month extracted from `travel_date`                   |
| `hour`              | Hour extracted from `travel_time`                    |

Additional engineered features and encodings were applied for better model learning.

---

## 🔍 Project Objectives

- Analyze demand patterns across different routes and times
- Predict the number of tickets for each trip using machine learning
- Provide insights into travel trends to assist fleet management decisions

---

## 🧠 Machine Learning Models Used

- Linear Regression
- Random Forest Regressor
- **XGBoost Regressor (Best performer)**

### ✅ Model Performance (XGBoost Regressor):
| Metric | Value |
|--------|-------|
| MSE    | 78.65 |
| RMSE   | 8.87  |
| R²     | 0.84  |

---

## 📊 Key Highlights

- 🧹 Data Cleaning and Preprocessing
- 🧠 Feature Engineering (Datetime extraction, label encoding)
- 📈 Exploratory Data Analysis & Visualization
- 🔁 Model Training, Tuning, and Evaluation
- 📦 Model Export (`joblib`)

---

## 🔮 Future Improvements

- Integrate external data like holidays, events, and weather
- Deploy the model via a web interface (Flask/Streamlit)
- Use time-series forecasting for more accurate trend analysis
- Optimize fleet dispatching using predicted demand

---

## 📁 Files Included





---

## 👨‍💻 Author

**Ravi**  
📧 Email: [ravishanka1819@gmail.com]  
🐙 GitHub: [https://github.com/ravishankar1810]  
🔗 LinkedIn: [https://www.linkedin.com/in/ravi-shankar-singh-08361b290/%5D]  

---
