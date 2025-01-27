# Parser Helper Challenge

Welcome to your Electricity Maps technical challenge! We have 45 minutes to attempt building a parser for load forecasts of the Califonian grid.

Most of California is covered by the [California ISO](https://app.electricitymaps.com/zone/US-CAL-CISO/72h/hourly). The name is abbreviated to `US-CAL-CISO` within Electricity Maps, but can be found as `CISO` or `CAISO` elsewhere. We've heard that the independent system operator (ISO) has a [data portal](https://www.caiso.com/Pages/default.aspx) where they publish load forecasts. We'd like to build a parser so that we can start ingesting these forecasts, turn them into features and improve our forecasting engine.

We're providing a notebook to gather your code, thoughts and answers.

## Setup

```bash
python -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

## Task 1 - Identify a data source

A competitor has access to forecasts for the California ISO, as demonstrated by their [data explorer](https://www.gridstatus.io/datasets).

Your first task is to:

1. Identify the dataset that holds load forecasts for the day-ahead market for the California ISO.
2. Identify the data source from which the dataset is derived.

## Task 2 - Find a way to download the data

Based on this data source, try to find a way to download a data sample as `.csv`.

## Task 3 - Propose a way to programmatically parse the data

Once you have a data sample, propose a way to programmatically parse the data into a format that is easy to work with.

## Task 4 - Implement the parser

Implement the parser in Python. If you've not have had time to build the parser, you can simply parse the .csv file attached here as `20250127_20250129_SLD_FCST_N_20250127_00_22_13_v1.csv`.
