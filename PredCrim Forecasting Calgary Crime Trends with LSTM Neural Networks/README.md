# CrimeCast: Predicting Calgary Crime Trends with LSTM

## 📌 Overview
**CrimeCast** is a data science and deep learning project aimed at analyzing and predicting monthly crime trends across Calgary communities. Using publicly available data from the City of Calgary (2018–2024), this project explores crime patterns and leverages an LSTM (Long Short-Term Memory) neural network for time-series forecasting.

## 🔍 Objectives
- Understand historical crime patterns across Calgary communities.
- Visualize and interpret community-wise and category-wise crime distributions.
- Build a neural network model to predict future crime counts.
- Support proactive crime prevention through data-driven forecasting.

---

## 🧠 Project Pipeline

1. **Data Acquisition & Understanding**  
   Load and explore Calgary Crime and Disorder data to assess structure and variables.

2. **Data Preprocessing**  
   Clean missing values, correct data types, and prepare time-series data sequences.

3. **Exploratory Data Analysis (EDA)**  
   Gain insights into crime distribution, trends, community hotspots, and seasonality.

4. **Model Development**  
   Build and train an LSTM-based neural network for monthly crime prediction.

5. **Model Evaluation & Forecasting**  
   Measure model performance and forecast future crime trends.

---

## 📊 Key Insights from EDA

### 🔴 Top Crime-Prone Communities:
- **Beltline**: Highest crime reports (11.4%)  
- **Forest Lawn**: 10.7%  
- **Downtown Commercial Core**: 10.2%

### 🟢 Safest Communities:
- **13M**: Only 22.7% of least crimes  
- **02K** and **02B**: 13.6% each

### 🚔 Common Crime Categories:
- Theft from Vehicle (21.7%)  
- Theft of Vehicle (16.7%)  
- Break & Enter – Commercial (13.8%)

### 📅 Yearly Trends:
- Highest reports in **2019**, followed by **2022** and **2018**  
- 2024 data is partial (early months only)

### 📆 Monthly & Seasonal Variations:
- Crime occurrences fluctuate seasonally, suggesting external triggers

---

## 🤖 Neural Network Model (LSTM)

### 📐 Architecture
- Input: Time-sequenced crime data  
- Layers:  
  - LSTM (50 units)  
  - Dropout (to prevent overfitting)  
  - Dense (final prediction output)  
- Loss: Mean Squared Error (MSE)  
- Optimizer: Adam

### 🏋️ Training Process
- Train/Test Split: Chronological
- Epochs: 100
- Validation Loss monitored to prevent overfitting

### 📈 Model Performance
- Training and validation loss decreased consistently
- Model effectively learned patterns for forecasting monthly crime counts

---

## ✅ Conclusion
**CrimeCast** showcases how deep learning and data analytics can offer powerful insights into urban safety. By predicting crime trends, such models can help city authorities optimize patrol planning, deploy resources efficiently, and make Calgary a safer place.

---

### 👨‍💻 Made with 💡 by **Surya Prakash**
