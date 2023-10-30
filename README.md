# Car-Sale-Exploratory-Data-Aanalysis

##Introduction

This code and guide provide an overview of how to perform time series analysis and visualization using Python libraries such as `geopandas`, `folium`, `scipy`, `matplotlib`, `seaborn`, and `statsmodels`. The analysis is demonstrated using a dataset containing information about vehicles listed on Craigslist. The code covers data preprocessing, visualization, and basic time series analysis techniques.

## Requirements

Before running the code, make sure you have the following Python libraries installed:

- geopandas
- folium
- scipy
- matplotlib
- seaborn
- statsmodels
- numpy
- pandas

You can install these libraries using pip:

```bash
!pip install geopandas folium scipy matplotlib seaborn statsmodels numpy pandas
```

## Getting Started

1. Download the dataset: Ensure you have a CSV file named 'craigslist_vehicles.csv' containing the dataset you want to analyze.

2. Import the necessary libraries at the beginning of your Python script or Jupyter Notebook:

```python
import os
import random
import geopandas as gpd
from shapely.geometry import Point
import folium
from scipy.stats import mode
import statsmodels.api as sm
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

3. Load the dataset using the pandas library:

```python
df = pd.read_csv('craigslist_vehicles.csv')
```

## Data Preprocessing

The code provides various data preprocessing steps, including:

- Dropping unnecessary columns.
- Handling missing values by filling categorical data with the mode and numerical data with the median.
- Converting date columns to datetime data types.
- Descriptive statistics of the dataset.

## Data Visualization

The code includes various data visualization techniques to explore the dataset:

- Visualizing the distribution of vehicle prices.
- Exploring relationships between price and features such as size, condition, type, transmission, and fuel.
- Creating bar plots and histograms to display the data.

## Time Series Analysis

The code performs basic time series analysis, including:

- Extracting month information from posting and removal dates.
- Grouping the data by months and visualizing the most posted listings and removals by month.

## Running the Code

You can run the code by copying it into a Python script or Jupyter Notebook. Ensure that you have the required libraries installed, and replace 'craigslist_vehicles.csv' with your dataset file if necessary.
