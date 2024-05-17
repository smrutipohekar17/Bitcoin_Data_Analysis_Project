# Bitcoin Price Analysis Project

## Overview

This project focuses on the analysis of Bitcoin price data from April 28, 2013, to July 31, 2017. It includes data pre-processing, visualizations, and identifying patterns or trends over time. The objective is to understand Bitcoin's historical price movements and provide insights into its market behavior.

## Table of Contents

- [Overview](#overview)
- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Data Description](#data-description)
- [Analysis Steps](#analysis-steps)
  - [Data Loading and Inspection](#data-loading-and-inspection)
  - [Data Pre-Processing](#data-pre-processing)
  - [Basic Data Analysis](#basic-data-analysis)
  - [Time Series Analysis](#time-series-analysis)
  - [Log-Scale Analysis](#log-scale-analysis)
  - [Resampling and Aggregation](#resampling-and-aggregation)
  - [Daily Return Analysis](#daily-return-analysis)
- [Visualizations](#visualizations)
- [Conclusion](#conclusion)
- [Contributing](#contributing)
- [License](#license)

## Project Structure

```
Bitcoin_Data_Analysis_Project/
│
├── data/
│   └── bitcoin_price_Training - Training.csv
│
├── notebooks/
│   └── bitcoin_price_analysis.ipynb
│
├── visualizations/
│   └── *.png
│
├── README.md
│
└── requirements.txt
```

## Getting Started

### Prerequisites

- Python 3.7+
- Jupyter Notebook or Jupyter Lab

### Installation

1. **Clone the repository**:
    ```sh
    git clone https://github.com/smrutipohekar17/Bitcoin_Data_Analysis_Project.git
    cd Bitcoin_Data_Analysis_Project
    ```

2. **Install the required libraries**:
    ```sh
    pip install -r requirements.txt
    ```

3. **Open the Jupyter Notebook**:
    ```sh
    jupyter notebook notebooks/bitcoin_price_analysis.ipynb
    ```

## Data Description

The dataset used in this project is `bitcoin_price_Training - Training.csv`, which contains the following columns:

- **Date**: The date of the record.
- **Open**: The opening price of Bitcoin on the given date.
- **High**: The highest price of Bitcoin on the given date.
- **Low**: The lowest price of Bitcoin on the given date.
- **Close**: The closing price of Bitcoin on the given date.

## Analysis Steps

### Data Loading and Inspection

- Load the dataset using Pandas.
- Preview the first few rows and inspect the structure of the dataset.

### Data Pre-Processing

- Convert the 'Date' column to datetime format.
- Check for missing values and duplicates.
- Sort the data in chronological order.

### Basic Data Analysis

- Compute descriptive statistics for price columns.
- Identify the date range covered by the dataset.

### Time Series Analysis

- Visualize the 'Open', 'High', 'Low', and 'Close' prices over time using line plots.
- Create a candlestick chart to visualize detailed price movements.

### Log-Scale Analysis

- Plot the closing price on a normal and logarithmic scale.
- Analyze upward trends and observe the absence of seasonality and outliers.

### Resampling and Aggregation

- Calculate and plot the average closing price on a yearly, quarterly, and monthly basis.

### Daily Return Analysis

- Calculate the daily return to understand day-to-day changes in closing prices.

## Visualizations

The project includes various visualizations to understand Bitcoin's price trends:

- Line plots of 'Open', 'High', 'Low', and 'Close' prices.
- Candlestick chart using Plotly.
- Yearly, quarterly, and monthly average closing prices.
- Logarithmic scale analysis of closing prices.

## Conclusion

This project provides a comprehensive analysis of Bitcoin price data, demonstrating proficiency in handling time series data, creating insightful visualizations, and extracting meaningful patterns from financial datasets.

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss your ideas.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
