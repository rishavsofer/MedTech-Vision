
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
3. **Install dependencies manually**:
   Run the following commands to install the required Python libraries:
   ```bash
   pip install yfinance
   pip install pandas
   pip install numpy
   pip install matplotlib
   pip install prophet
   ```
   These libraries are required for data handling, analysis, visualization, and forecasting.

4. **Run the script**:
   ```bash
   python "MedTech_Vision.py"
   ```
   This script will download the data, build the index, backtest it, and generate a 90-day forecast.

## Usage

- **Adjust Tickers**: Open `MedTech_Vision.py` and edit the `tickers` list to include/exclude specific stocks.
- **Modify Forecast Period**: Update the Prophet `make_future_dataframe(periods=90)` line to forecast more or fewer days.
- **Customize Parameters**: You can fine-tune Prophet hyperparameters or modify index construction logic within the script.

## Results and Interpretation

- The script generates key metrics like total return, annualized return, and volatility.
- Prophet's trend and seasonality plots are displayed automatically.
- Use these insights to explore the MedTech sector's performance and make data-driven predictions.

## Contributing

Contributions are welcome! Fork the repository, make your changes, and submit a pull request.

## License

This project is provided under the [MIT License](LICENSE). Feel free to use, share, and adapt the code for your own purposes.

## Contact

- **Email**: [rishavlincoln@gmail.com](mailto:rishavlincoln@gmail.com)

Happy forecasting!
