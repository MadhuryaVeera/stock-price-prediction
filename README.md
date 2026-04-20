# Stock Price Prediction Using Machine Learning Using LSTM & GRU.

A final-year project that predicts stock prices for selected Indian banking stocks using multiple models (ARIMA, LSTM, GRU, and Stacked LSTM) and serves results through a Flask web application.

## Problem Statement
Stock market prices are highly dynamic and difficult to forecast manually. Traditional analysis methods are often not enough to handle non-linear, time-dependent financial data. This project aims to build a practical prediction system that compares classical time-series modeling and deep learning approaches to estimate future stock prices for major banking stocks and present the results in a user-friendly web interface.

## Project Objectives
- Predict future stock values using trained models.
- Compare model performance using metrics such as MSE, RMSE, MAE, and R2.
- Provide a web UI for user login, model comparison, and forecast visualization.
- Support multi-bank forecasting (for example: SBIN, HDFCBANK, AXISBANK, ICICIBANK, INDUSINDBK).

## Tech Stack
- Language: Python
- Backend Framework: Flask
- Frontend: HTML, CSS, JavaScript, Bootstrap
- Database: MySQL
- Data/ML Libraries:
  - pandas, numpy
  - scikit-learn
  - statsmodels (ARIMA)
  - TensorFlow/Keras (LSTM, GRU, Stacked LSTM)
  - matplotlib
  - joblib
- Model/Data Artifacts:
  - .h5 (deep learning models)
  - .pkl (scalers and ARIMA artifacts)
  - .csv (datasets and outputs)
- Models that i used in this is :
   - LSTM
   - Stacked LSTM
   - GRU
   - ARIMA
   

## Project Structure
```text
TK200773-Stock Price Prediction/
├── TK197036-Stock Price Prediction/
│   ├── Abstract/
│   ├── Code/
│   │   ├── Backend/
│   │   │   ├── code.ipynb
│   │   │   ├── *.h5, *.pkl, *.csv
│   │   │   └── evaluation plots
│   │   └── Frontend/
│   │       ├── app.py
│   │       ├── db.sql
│   │       ├── templates/
│   │       └── static/
│   ├── Document/
│   ├── ppt/
│   └── Video/
└── README.md
```

## Main Modules
- User Authentication: Register and login pages backed by MySQL.
- Algorithm Comparison: Displays performance values for each model and bank.
- Prediction Module: Generates future-day predictions and forecast plots.
- Result/About Pages: Shows output summaries and project information.

## How To Run
1. Clone the repository.
2. Go to the frontend app directory:
   - TK197036-Stock Price Prediction/Code/Frontend
3. Create and activate a Python virtual environment.
4. Install required packages:
   - flask
   - mysql-connector-python
   - pandas
   - numpy
   - scikit-learn
   - joblib
   - matplotlib
   - statsmodels
   - tensorflow
5. Create a MySQL database named stock.
6. Import schema from db.sql.
7. Update MySQL credentials in app.py if needed.
8. Run the app:
   - python app.py
9. Open the local Flask URL shown in terminal (usually http://127.0.0.1:5000).



## Notes
- The project already includes trained model files and scaler files for supported banks.
- Forecast plots are generated under the static folder when predictions are made.
- The app currently runs in debug mode in app.py.

## Future Improvements
- Add model retraining pipeline from live market data.
- Add secure password hashing and session management.
- Add API endpoints for programmatic prediction access.
- Add Docker support and deployment configuration.

## Repository
GitHub: https://github.com/MadhuryaVeera/stock-price-prediction
