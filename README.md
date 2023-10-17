# StockX Market Data Analysis (2020-2021)

This repository contains a comprehensive dataset of daily market data scraped from StockX for over 4000 top products from 2020 to 2021. With over 1 million entries, this dataset aims to provide insights into market dynamics, price trends, and buyer-seller behaviors on the StockX platform.

## Dataset Description

The dataset comprises daily market snapshots for a variety of products, captured in JSON format. Each entry includes the following fields:

- `ID`: Unique identifier for each product.
- `date`: Timestamp of the data collection.
- `lowestAsk`: Lowest asking price on the market.
- `highestBid`: Highest bid price on the market.
- `numberOfAsks`: Total number of asks on the market.
- `numberOfBids`: Total number of bids on the market.
- `deadstockSold`: Number of deadstock items sold.
- `totalDollars`: Total transaction value in dollars.
- `pricePremium`: Price premium percentage.

## Installation

1. Clone the repository:
```bash
git clone https://github.com/Flurin17/stockXsalesData.git


## Usage
import pandas as pd
import matplotlib.pyplot as plt

# Load the dataset
data = pd.read_json('data/stockx_market_data.json', lines=True)

