# Stock Price Prediction (Short-Term)

## Task 2: Predict Future Stock Prices

### Objective
The objective of this project is to use historical stock market data to predict the **next day’s closing price** of a stock. This project demonstrates how machine learning models can be applied to financial time-series data for short-term price prediction.

---

### Dataset
The dataset is retrieved directly from **Yahoo Finance** using the `yfinance` Python library.  
It contains historical stock price data including:

- Open price  
- High price  
- Low price  
- Close price  
- Trading volume  

**Example stocks used:**  
- Apple Inc. (AAPL)  
- Tesla Inc. (TSLA)  

---

### Project Instructions
The following steps were performed in this project:

1. **Stock Selection**
   - Selected a publicly traded company (e.g., Apple or Tesla).

2. **Data Collection**
   - Loaded historical stock data using the `yfinance` library.

3. **Feature Selection**
   - Used the following features as input variables:
     - Open
     - High
     - Low
     - Volume
   - Target variable:
     - Next day’s **Close** price

4. **Model Training**
   - Trained machine learning models such as:
     - **Linear Regression**
     - **Random Forest Regressor**

5. **Model Evaluation**
   - Evaluated the model using regression metrics such as:
     - R² Score
     - Visual comparison of predictions

6. **Visualization**
   - Plotted **actual vs predicted closing prices** to visually analyze model performance.

---

### Tools and Libraries
- Python 3.x  
- Libraries used:
  - `yfinance`
  - `pandas`
  - `numpy`
  - `matplotlib`
  - `scikit-learn`
