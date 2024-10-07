# Flight Radar 24 Project

## Objective
This project aims to process and analyze airport and flight data in real-time using Apache Spark. The system is designed to handle large-scale datasets generated from sources like FlightRadar.

## Overview
The project involves developing a scalable solution for ingesting, processing, and analyzing airport and flight data. Key performance indicators (KPIs) will be computed, including average flight speeds and delayed flights, using various Spark operations.

## Datasets
The project utilizes the following datasets:
- `adsb.json`: Contains ADS-B flight data.
- `oag.json`: Contains OAG flight data.

### Schema Information
The following schema files describe the structure of the datasets:
- `adsb_schema.json`: Defines the structure of `adsb.json`, which includes fields such as `AircraftId`, `Flight`, `LastUpdate`, `Speed`, etc.
- `oag_schema.json`: Defines the structure of `oag.json`, which contains flight schedules and additional metadata related to airport operations.

These schema files provide detailed information on the fields, data types, and whether the fields are nullable or required. You can find the schema files in the project root directory:
- [adsb_schema.json](./adsb_schema.json)
- [oag_schema.json](./oag_schema.json)

## Features
- Load and process large datasets using Apache Spark.
- Clean and transform data to extract relevant information.
- Calculate airport KPIs:
  - Average speed for each airport.
  - Total number of delayed flights (arrival and departure).
- Apply window functions to filter and retain the most recent entries for each FlightId.
- Present results in graphical or tabular format.

## Requirements
This project includes Jupyter notebooks `flightRadar24Project.ipynb` to explore and analyze the datasets interactively. 

To run this project, you need to install the following dependencies:

- Python 3.x
- Additional Python packages listed in `requirements.txt`

### Install Dependencies
You can install the required dependencies using the following command:

```bash
pip install jupyter
pip install -r requirements.txt


