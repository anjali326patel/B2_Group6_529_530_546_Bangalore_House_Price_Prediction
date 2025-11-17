# Bangalore_house_price_predictor
Bangalore_House_Price_Prediction
A Machine Learning–Powered Web Application for Real Estate Price Estimation

1. Project Overview
Bangalore_House_Price_Prediction is an end-to-end Data Science & Web Development project that predicts housing prices across various localities in Bengaluru.
The system integrates:
🔹 Data preprocessing
🔹 Feature engineering
🔹 Outlier removal
🔹 Machine learning regression
🔹 Flask API backend
🔹 Interactive frontend (HTML/CSS/JS)
🔹 Real-time price comparison
🔹 Market value meter (undervalued / fair price / overpriced)
This project demonstrates a complete lifecycle of a real-world ML deployment system.

Developed By
> Anjali Patel
> Disha Janve
> Kanchan Jadhav

2. Features Implemented
   
🔹 Machine Learning
Linear Regression–based prediction model
Location-wise one-hot encoding (240+ locations)
Automatic outlier detection & removal
sqft & BHK normalization
Final model saved as pickle for deployment

🔹 Data Preprocessing
Missing value handling
Converting categorical features
Creating price_per_sqft feature
Removing inconsistent entries
Removing BHK & bathroom outliers
Removing location-based deviations (SD filtering)

🔹 Backend (Flask API)
/api/predict_home_price → returns predicted price
/api/get_location_names → returns location list
/api/location_stats → returns median, low_5, high_95

🔹 Frontend
Clean UI with modern blurred-glass background
Single location price estimator
Multi-location comparison (2–5 locations)
Bar chart comparison (Chart.js)
Market value meter:
Green → undervalued
Yellow → fair
Red → overpriced
Responsive layout (left estimator + right comparison)

3. System Architecture (Figures Overview)

📘 Figure 1 — Overall System Architecture
Shows full pipeline:
Dataset → Cleaning → Feature Engineering → Model Training → Pickle Model → Flask API → Frontend UI.

📘 Figure 2 — Data Preprocessing Workflow
Illustrates:
Missing value handling
BHK extraction
sqft conversion
price_per_sqft
Outlier removal (IQR + SD + BHK logic)

📘 Figure 3 — Deployment Architecture
Frontend (HTML/CSS/JS) ↔ Flask Server ↔ ML Model ↔ JSON Response

4. Project Structure
Bangalore_House_Price_Prediction/
│
├── client/
│   ├── app.html
│   ├── app.css
│   ├── app.js
│   └── assets/
│
├── artifacts/
│   ├── banglore_home_prices_model.pickle
│   ├── columns.json
│   └── location_stats.json (embedded inside columns.json)
│
├── server.py
├── util.py
├── model_training_notebook.ipynb
└── README.md

5. Tech Stack
Machine Learning

Python
-NumPy
-Pandas
-scikit-learn
-Matplotlib / Seaborn

Deployment
-Flask
-Ngrok / Google Colab Proxy
-Pickle Model Serialization

Frontend
-HTML5
-CSS3
-JavaScript
-Chart.js

6. Model Performance

R² Score (Linear Regression): 0.85+
RMSE: Low deviation after outlier removal
Outlier removal significantly improved model stability and interpretability.

7. Demonstration (Key Screens)

Single price prediction
Multi-location comparison
Bar chart visualization
Market meter indicator
<img width="1920" height="961" alt="Screenshot (25)" src="https://github.com/user-attachments/assets/8c69da90-9c32-44bd-ad99-36aa2603a5ab" />
<img width="1920" height="957" alt="Screenshot (26)" src="https://github.com/user-attachments/assets/e77aa06f-be52-41ab-b7bc-705855807bc8" />

8. Conclusion

This project successfully delivers a full-stack ML system capable of predicting and comparing real estate prices with strong accuracy and clean UI.
It demonstrates mastery of:

✔ Data preprocessing
✔ ML model building
✔ API development
✔ Frontend integration
✔ Visualization
✔ Market analytics

A complete showcase of modern applied Data Science.
