# Stock Price Predictor

## IEEE TEMS Junior Recruitment Task

This project implements a stock price prediction system using machine learning techniques. It demonstrates the application of time series analysis and deep learning to predict future stock prices based on historical data.

### Project Overview

The project uses both traditional statistical methods and modern deep learning approaches to predict stock prices. It includes:

- Data collection using yfinance API
- Comprehensive data preprocessing and feature engineering
- Implementation of an LSTM (Long Short-Term Memory) neural network
- Model evaluation using RMSE and visualization
- Next-day price prediction capability

### Technical Stack

- Python 3.8+
- Key libraries:
  - yfinance: For fetching historical stock data
  - pandas: For data manipulation and analysis
  - numpy: For numerical computations
  - scikit-learn: For data preprocessing and metrics
  - tensorflow: For implementing the LSTM model
  - matplotlib & seaborn: For data visualization

### Project Structure

```
stock-price-predictor/
├── stock_price_predictor.ipynb    # Main Jupyter notebook with all the code and analysis
└── README.md                      # Project documentation
```

### Setup Instructions

1. Clone the repository:
   ```bash
   git clone [your-repository-url]
   cd stock-price-predictor
   ```

2. Install required packages:
   ```bash
   pip install yfinance pandas numpy matplotlib seaborn scikit-learn tensorflow
   ```

3. Open and run the Jupyter notebook:
   ```bash
   jupyter notebook stock_price_predictor.ipynb
   ```

### Technical Decisions

1. **Data Source**: Chose yfinance for its reliability and ease of use in fetching historical stock data.

2. **Feature Engineering**:
   - Implemented technical indicators like Moving Averages, RSI, and Bollinger Bands
   - Used a 60-day lookback period for sequence prediction

3. **Model Architecture**:
   - Used LSTM for its ability to capture long-term dependencies in time series data
   - Implemented dropout layers to prevent overfitting
   - Used MinMaxScaler for feature scaling

4. **Evaluation Metrics**:
   - Root Mean Square Error (RMSE) for model performance evaluation
   - Visual comparison of predicted vs actual prices

### Challenges and Solutions

1. **Data Preprocessing**:
   - Challenge: Handling missing values and outliers
   - Solution: Implemented robust data cleaning techniques and rolling windows for feature calculation

2. **Model Training**:
   - Challenge: Preventing overfitting
   - Solution: Added dropout layers and used appropriate validation split

3. **Prediction Accuracy**:
   - Challenge: Balancing model complexity with performance
   - Solution: Fine-tuned hyperparameters and implemented multiple technical indicators

### Future Improvements

1. Implement ensemble methods combining multiple models
2. Add more advanced technical indicators
3. Include sentiment analysis from news and social media
4. Develop a web interface for real-time predictions

### License

This project is licensed under the MIT License - see the LICENSE file for details.

