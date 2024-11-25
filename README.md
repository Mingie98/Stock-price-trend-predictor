# Stock Price Prediction using LSTM

## Project Overview
This project leverages a Long Short-Term Memory (LSTM) neural network to predict future stock prices based on historical price data. This deep learning model is implemented in Python with Keras and TensorFlow libraries.

## Features
- **Data Collection**: Collect historical stock price data through an API call.
- **Data Preprocessing**: Normalizes and sequences stock price data for better model performance.
- **LSTM Network**: Utilizes a sequential model of LSTM layers to learn from historical prices.
- **Visualization**: Plots training and testing predictions against actual stock prices.
- **Evaluation**: Calculates Root Mean Square Error (RMSE) to assess model accuracy.

## Results
The vanilla RNN model struggled with the task, displaying poor predictive value.
On a 30-day prediction, the model overshot the stock price by nearly $20 on the last day, showing significant inaccuracies.
- ![image](https://github.com/user-attachments/assets/1c183199-778c-4793-b737-e614aa951458)

The LSTM model performed significantly better.
It correctly predicted the overall direction of the trend during the 30-day period, although it wasn't perfect.
- ![image](https://github.com/user-attachments/assets/998a8478-0811-4573-85f7-42ee5c6da4ce)

## Shortcomings 
- Variability in Results: The LSTM model produced inconsistent predictions during repeated runs, making its reliability questionable.
- Occasional Poor Performance: In certain instances, the LSTM model performed worse than the simpler RNN model.
- Lack of Feature Diversity: The model only relied on historical prices, ignoring other potential predictive features such as trading volume, technical indicators, or external factors like news sentiment.
- Evaluation Limitation: RMSE, while useful, may not fully capture the economic relevance or profitability of predictions in a trading context.

