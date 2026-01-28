# Smart Energy Consumption Forecasting

## Overview
This project focuses on forecasting household electricity consumption using time-series analysis and machine learning techniques. The objective is to analyze historical energy usage data, identify trends and seasonal patterns, and build predictive models for future consumption.

The project follows a complete data science workflow, including data preprocessing, exploratory analysis, statistical modeling, and machine learning-based forecasting.

---

## Dataset
The project uses a public household electricity consumption dataset containing historical power usage measurements.

⚠️ **Note:**  
The dataset is not included in this repository due to size constraints.  
To run the notebook locally, download the dataset separately and place it in a `data/` folder.

---

## Methodology

### 1. Data Preprocessing
- Converted date and time into a proper datetime index
- Handled missing values using time-based interpolation
- Resampled minute-level data into daily average consumption

### 2. Exploratory Data Analysis (EDA)
- Visualized long-term trends using rolling averages
- Performed seasonal decomposition (trend, seasonality, residual)
- Analyzed monthly consumption patterns

### 3. Stationarity Testing
- Applied Augmented Dickey–Fuller (ADF) test
- Used first-order differencing to achieve stationarity

### 4. Forecasting Models
- **ARIMA (1,1,1)** model for time-series forecasting
- **Random Forest Regression** using lag-based features for machine learning comparison

### 5. Model Evaluation
- Evaluated models using MAE and RMSE
- Compared statistical and machine learning approaches

---

## Tools & Technologies
- Python
- pandas, numpy
- matplotlib
- statsmodels
- scikit-learn
- Jupyter Notebook

---

## Results
The analysis revealed clear trend and seasonal patterns in electricity consumption.  
The ARIMA model provided a strong baseline forecast, while the Random Forest model demonstrated the ability to capture non-linear relationships. The comparison highlights the trade-offs between interpretability and computational complexity.

---

## Conclusion
This project demonstrates how both time-series and machine learning models can be applied to real-world energy consumption forecasting. The methodology and results provide a solid foundation for further extensions such as advanced seasonal models, external feature integration, or deep learning approaches.

---

## Future Scope
- Incorporating weather and calendar data
- Seasonal ARIMA (SARIMA) modeling
- Deep learning models such as LSTM
- Real-time energy demand forecasting
