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
│   └── Bitcoin_Data_Analysis.ipynb
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

## Key Insights::

- Historical Price Movements: Identify significant trends and patterns in the historical price data of Bitcoin.
- Data Visualization: Effective use of visualizations to convey price trends, with tools like line plots and candlestick charts.
- Logarithmic Scaling: Demonstrate the utility of log scales in handling datasets with wide-ranging values.
- Temporal Analysis: Understand price trends on various time scales (yearly, quarterly, monthly).

## Tools and Techniques:

- Pandas: For data manipulation and pre-processing.
- Numpy: For numerical computations.
- Matplotlib and Seaborn: For creating static visualizations.
- Plotly: For interactive visualizations, particularly the candlestick chart.
- Datetime Conversion: Ensuring the 'Date' column is in the correct format for time series analysis.
- Resampling: Aggregating data on different time scales (yearly, quarterly, monthly).

## Conclusion

This project serves as a comprehensive exercise in analyzing Bitcoin price data, employing various data processing techniques, visualizations, and temporal aggregations. It helps in deriving meaningful insights from historical data, which could be useful for understanding market trends and making informed decisions. As a data analyst, such a project demonstrates proficiency in handling time series data, data visualization, and extracting actionable insights from financial datasets.

## Contributing

Contributions are welcome! Please create a pull request or open an issue to discuss your ideas.

