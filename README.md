# 🌍 Weather Trend Forecasting

Welcome to my project on **climate forecasting using machine learning**, where I explore and model global temperature trends using weather and air quality data.  
The goal of this project is to **predict temperature (in Celsius)** based on various environmental factors.

---

## 📁 Project Structure

```
📦 Weather_Trend_Forecasting
├── 📄 Model.ipynb   # Main notebook with complete EDA, modeling & analysis
├── 📄 requirements.txt        
├── 📄 best_model.h5                        # Saved LSTM model weights (best performing model)
├── 📄 report.pdf            # Detailed report outlining methodology & findings
├── 📄 README.md                            # Project overview and documentation (this file)
```
---
## 🧾 How to Use This Repo

### 🔻 Clone the repository
```bash
git clone https://github.com/isha-harish/Weather_Trend_Forecasting.git.
cd Weather_Trend_Forecasting
```
### 📦 Install dependencies
```bash
pip install -r requirements.txt

```

### 🚀 Launch the notebook
Get Data from : https://www.kaggle.com/datasets/nelgiriyewithana/global-weather-repository/code
Open Model.ipynb in Jupyter Notebook or Jupyter Lab and run the cells to explore the analysis and model results.

---

## 📊 Data Overview

The dataset `GlobalWeatherRepository.csv` includes features such as:

- **Weather metrics**: humidity, pressure, UV index, wind speed, wind direction  
- **Air quality metrics**: PM2.5, PM10, CO, O3, NO2, SO2  
- **Astronomical info**: sunrise, sunset, moonrise, moonset, moon phase  
- **Location & geographic coordinates**  
- **Target**: `temperature_celsius`  

---

## 🧪 Exploratory Data Analysis (EDA)

Performed a thorough EDA including:

- 📈 Time Series Analysis of temperature and pollutants  
- 🗺️ Geographical Visualization of temperature distribution  
- 🔥 Feature Importance using Random Forest  
- 🧼 Missing value treatment & normalization  
- 🌡️ Correlation Analysis between temperature & air quality  
- ⚠️ Outlier Detection  
- 🔍 Time decomposition for trend/seasonality analysis  

---

## 🤖 Machine Learning Models

Three different models were built to forecast temperature:

### 1️⃣ Random Forest Regressor
- Robust tree-based ensemble model for regression  
- Evaluated using MAE, MSE, R²  

### 2️⃣ XGBoost Regressor
- Gradient boosting model optimized for speed and accuracy  
- Great for structured tabular data  

### 3️⃣ LSTM (Long Short-Term Memory)
- Deep learning model ideal for time-series forecasting  
- Used TensorFlow/Keras  
- Saved as `best_model.h5` using EarlyStopping & ModelCheckpoint  

---

## 🧠 Ensemble Learning

Two ensemble strategies were used to improve performance:

- ✅ **Simple Average**: Mean of predictions from all three models  
- ✅ **Weighted Average**: Models weighted based on inverse MAE (lower error = higher weight)  

---

## 📈 Evaluation Metrics

All models were evaluated on the validation set using:

- **MAE**: Mean Absolute Error  
- **MSE**: Mean Squared Error  
- **R² Score**: Goodness of Fit  

---
## 🛠️ Tech Stack

- **Python:** Pandas, NumPy, Scikit-learn, TensorFlow, XGBoost

- **Visualization:** Matplotlib, Seaborn

- **Modeling:** RandomForest, XGBoost, LSTM

- **Notebook:** Jupyter (.ipynb)

---
