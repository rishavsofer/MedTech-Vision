```markdown
# MedTech Vision

MedTech Vision is a Python-based project that constructs an equal-weighted index from five major MedTech stocks—MDT, JNJ, SMMNY, SYK, and GEHC—then backtests the index’s historical performance and forecasts 90-day trends using Prophet.

## Features

- **Data Retrieval:** Fetch daily historical price data via `yfinance`.
- **Index Construction:** Create an equal-weighted custom MedTech index.
- **Backtesting:** Plot the index performance over the last two years and compute basic metrics (return, volatility).
- **Forecasting:** Use Prophet to predict the next 90 days of index movement.
- **Visualization:** Generate charts for historical performance, Prophet’s trend forecast, and seasonality components.

## Getting Started

1. **Clone the repository**:
   ```bash
   git clone https://github.com/YourUsername/MedTech-Vision.git
   cd MedTech-Vision
   ```
2. **Set up a virtual environment** (optional, but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```
3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the main script**:
   ```bash
   python main.py
   ```
   This script will download the data, build the index, backtest it, and generate a 90-day forecast.

## Project Structure

```plaintext
MedTech-Vision/
│
├── main.py               # Main workflow script
├── requirements.txt      # Project dependencies
├── README.md             # Project documentation
└── src/
    ├── data_retrieval.py # Functions to fetch price data
    ├── index_builder.py  # Logic to build the equal-weighted index
    ├── backtest.py       # Backtest metrics and plotting
    ├── forecast.py       # Prophet model training and forecast
    └── plots.py          # Visualization utilities
```

## Usage

- **Adjust Tickers**: In `main.py` (or within `src/index_builder.py`), edit the `tickers` list to include/exclude specific stocks.
- **Modify Forecast Period**: In `src/forecast.py`, change `periods=90` to forecast more or fewer days.
- **Hyperparameter Tuning**: Fine-tune the Prophet model (e.g., `seasonality_mode`, `changepoint_prior_scale`) or experiment with other libraries like ARIMA, LSTM, or XGBoost.

## Results and Interpretation

- The script prints key backtest metrics (annualized return, volatility) to the console.
- Prophet plots (trend, seasonality) are displayed automatically.
- Use these insights to compare MedTech’s performance with other benchmarks or for deeper strategic decisions.

## Contributing

Contributions are welcome!  
- Fork the repo  
- Create a new branch (`git checkout -b feature/YourFeature`)  
- Commit changes (`git commit -am 'Add a cool feature'`)  
- Push to the branch (`git push origin feature/YourFeature`)  
- Open a Pull Request  

Please open an issue if you have any questions or ideas.

## License

This project is provided under the [MIT License](LICENSE). Feel free to use, share, and adapt the code for your own purposes.

## Contact

- **Email**: [rishavlincoln@gmail.com](mailto:rishavlincoln@gmail.com)

Happy forecasting!
```




