# MetroPT3 Air Compression Optimization

## Project Overview

This project analyzes and optimizes the air compression system used in metro operations by leveraging historical data and predictive analytics. It aims to enhance system reliability, reduce maintenance costs, and improve overall performance through data-driven insights.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Cleaning](#data-cleaning)
- [Predictive Analysis](#predictive-analysis)
- [Classification Report Interpretation](#classification-report-interpretation)
- [Visualizations](#visualizations)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

MetroPT3 is an air compression system used in metro operations, which plays a crucial role in maintaining the functionality and efficiency of metro transit systems. Proper optimization of air compression operations is vital to ensure reliability, reduce maintenance costs, and enhance system performance. This project aims to analyze and optimize the air compression system by leveraging historical data and predictive analytics.

## Dataset

The dataset used in this project includes the following columns:
- `Index`
- `timestamp`
- `TP2`
- `TP3`
- `H1`
- `DV_pressure`
- `Reservoirs`
- `Oil_temperature`
- `Motor_current`
- `COMP`
- `DV_electric`
- `Towers`
- `MPG`
- `LPS`
- `Pressure_switch`
- `Oil_level`
- `Caudal_impulses`

## Exploratory Data Analysis (EDA)

### Sweetviz Report

Exploratory Data Analysis (EDA) is a crucial step in understanding the dataset, identifying trends, and uncovering insights. To facilitate this process, we use Sweetviz, a Python library that generates comprehensive and visually appealing EDA reports.

Sweetviz is a powerful library for generating visualizations and summary statistics for datasets. It provides a quick overview of data distributions, comparisons between datasets, and insights into correlations and missing values. This tool is particularly useful for gaining an initial understanding of the dataset and identifying patterns that might warrant further investigation.

```python
import sweetviz as sv

# Load your dataset
data = pd.read_csv('/content/drive/MyDrive/metro dataset for predictive maintenance /MetroPT3(AirCompressor).csv')

# Create and display the Sweetviz report
report = sv.analyze(data)
report.show_html('EDA_Report.html')







