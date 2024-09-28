# Investment-Portfolio-Tracker

This repository contains an investment portfolio tracker program that provides real-time stock information obtained from Yahoo Finance. The program is designed to automate the process of tracking investments using only transaction logs. Users no longer need to manually calculate their average price or track portfolio performance. By simply providing raw transaction history data, the program automatically calculates key metrics such as average purchase price, current holdings, realized gains, and overall returns.

## Project Structure

1. **Transaction History**
    - Reads raw transaction logs from an Excel file.
    - Adjusts transaction history for stock splits that occur after the first transaction date.

2. **Average Stock Price**
    - Calculates average stock purchase price using the FIFO cost basis method.

3. **Realized Profit of Traded Stocks**
    - Calculates realized profit of sold stocks using the FIFO cost basis method.

4. **Portfolio Summary**
    - Summarizes real-time portfolio information in a table.
    - Visualizes asset allocation and portfolio value using a pie chart.

5. **Unrealized Profit of Portfolio**
    - Reports unrealized portfolio returns.
    - Visualizes the unrealized profit of each stock using a bar chart.

## Library Installation

This project uses Yahoo! Finance API to fetch market data using the [yfinance](https://pypi.org/project/yfinance/) Python library.
To install the library, use the command line to deploy the installation from [PyPI](https://pypi.org) using pip.
```sh
$ pip install yfinance --upgrade --no-cache-dir
```

## Running the Code

To run the portfolio tracker, follow these steps:

1. Install [TransactionHistory.xlsx](TransactionHistory.xlsx) and edit the transaction logs according to your investments (**DO NOT** change the header row or delete any columns).
2. Edit the file directory of the Excel file in the first line of the 2nd cell of the notebook.
3. Execute all cells in the notebook in sequential order.

## License

[MIT](LICENSE) © 2024 Caitlyn Kay
