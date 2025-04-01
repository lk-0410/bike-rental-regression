# 🚴‍♀️ Bike Rental Demand: Regression Analysis Project

## 📌 Overview
This project analyzes a bike sharing dataset to predict the total number of daily rentals (`cnt`) based on variables like temperature, humidity, season, and weather. We use linear regression techniques and apply diagnostic tools to improve model performance and stability.

## 📊 Dataset
- **Source**: UCI Bike Sharing Dataset
- **Link**: [Bike Sharing Dataset](https://archive.ics.uci.edu/ml/datasets/Bike+Sharing+Dataset)
- **Rows**: 731 days of data
- **Target**: `cnt` (total number of rentals per day)

## 🛠 Tools & Libraries Used
- **R & RMarkdown**
- `dplyr`, `ggplot2`, `car`, `lmtest`, `corrplot`, `caret`, `MASS`

## 🔬 Key Features Explored
- `temp`, `hum`, `windspeed`
- `season`, `weathersit` (weather situation)
- `holiday`, `workingday`

## 📈 Techniques Used
- Multiple Linear Regression
- Log Transformation of target variable
- Residual Analysis & Q-Q Plots
- Breusch-Pagan Test for heteroscedasticity
- Stepwise Model Selection (AIC)

## ✅ Model Improvements
| Metric                      | Original Model | Log-Transformed Model |
|----------------------------|----------------|------------------------|
| Adjusted R²                | 0.5535         | **0.5839**             |
| Residual Std. Error        | 1294           | **0.3758**             |
| Breusch-Pagan p-value      | Very small     | Slightly better        |

## 💡 Findings
- `temp`, `hum`, and `windspeed` are significant predictors.
- Seasonal variation impacts rental volume.
- Log transformation improves the model fit and reduces error.
- Some heteroscedasticity remains even after transformation.

## 📂 Project Structure
```
bike-rental-regression/
├── data/
│   └── day.csv (not uploaded)
├── notebooks/
│   └── Regression-Project.Rmd
├── reports/
│   └── Regression-Project.html
├── images/
│   └── correlation_matrix.png
│   └── qq_plot.png
├── README.md
```

## 📸 Visuals
### 🔵 Correlation Matrix
![Correlation Matrix](images/correlation_matrix.png)

### 🔵 Q-Q Plot
![QQ Plot](images/qq_plot.png)

---

## 🤝 Author
**Lava**  
📅 *Project Date: Nov 15, 2024*

---

## 📬 Let's Connect
Feel free to connect on [LinkedIn](https://www.linkedin.com/) or reach out via email!
