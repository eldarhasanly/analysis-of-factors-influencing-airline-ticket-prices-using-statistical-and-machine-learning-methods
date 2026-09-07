# Dataset

This project uses the **Airline Market Fare Prediction Data** dataset created by **K. Gülnaz Bülbül** and published on Mendeley Data.

## Source

* **Dataset:** Airline Market Fare Prediction Data
* **Author:** K. Gülnaz Bülbül
* **Version:** 2
* **Published:** May 15, 2025
* **DOI:** `10.17632/m5mvxdx2wp.2`
* **Source:** https://data.mendeley.com/datasets/m5mvxdx2wp/2
* **License:** CC BY-NC 4.0

The dataset is derived from publicly available data provided by the **U.S. Department of Transportation Bureau of Transportation Statistics (BTS)**. It combines processed data from the **DB1B** and **T-100** datasets and includes additional variables describing market competition, route characteristics, and airport structure.

## Dataset Overview

The dataset contains:

* **1,581,278 observations**
* **26 variables**
* **Target variable:** `Average_Fare`

The variables describe airline markets, routes, carriers, passenger volumes, competition, and fare characteristics.

Selected explanatory variables include:

| Variable        | Description                            |
| --------------- | -------------------------------------- |
| `NonStopMiles`  | Non-stop route distance                |
| `MktMilesFlown` | Market miles flown                     |
| `Pax`           | Passenger volume                       |
| `CarrierPax`    | Carrier passenger volume               |
| `Market_share`  | Carrier market share                   |
| `Market_HHI`    | Market concentration                   |
| `LCC_Comp`      | Low-cost carrier competition indicator |
| `Multi_Airport` | Multiple-airport market indicator      |
| `Circuity`      | Route circuity                         |
| `Non_Stop`      | Non-stop service indicator             |

The dataset also contains encoded identifiers for markets, airports, carriers, and origin-destination pairs, together with frequency-encoded versions of several identifiers.

## Local Setup

The raw dataset is not stored in this GitHub repository because the CSV file is approximately **382 MB**.

To reproduce the analysis:

1. Download Version 2 of the dataset from the Mendeley Data source above.
2. Place `MarketFarePredictionData.csv` inside this directory.

The expected structure is:

```text
data/
├── README.md
└── MarketFarePredictionData.csv
```

The analysis notebook loads the dataset from:

```text
../data/MarketFarePredictionData.csv
```

The CSV file is excluded from version control through `.gitignore`.

## Data Usage

This project uses only publicly available data. No confidential or proprietary data from Azerbaijan Airlines or any other airline is included.

The dataset is distributed under the **Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)** license. Please refer to the original Mendeley Data record for the applicable licensing terms.