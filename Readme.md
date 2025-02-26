# Web Scraping and Data Collection from Truck Suvidha

## Overview
This project automates the collection of load details from the Truck Suvidha website, enriches it with geographical data, and stores it periodically. The script extracts the data, adds timestamps, fetches latitude and longitude of destination cities, and saves it in CSV files for further analysis.

## Features
- Scrapes load details from the Truck Suvidha website using `pandas.read_html()`.
- Appends data to a CSV file with timestamps for historical tracking.
- Uses `geopy` to fetch latitude, longitude, and population of destination cities.
- Runs automatically every 10 minutes using `schedule`.

## Requirements
- Python 3.x
- Required libraries:
  - `pandas`
  - `datetime`
  - `os`
  - `schedule`
  - `time`
  - `geopy`

## Installation
Ensure you have the necessary libraries installed by running:
```sh
pip install pandas schedule geopy
```

## Usage
1. Run the script to start scraping and storing data:
```sh
python script.py
```
2. The extracted data will be saved as:
   - `trucksuvidha_data.csv`: Contains load details with timestamps.
   - `destination_data.csv`: Contains geographical details of destination cities.

## Output
- A continuously updating dataset of load details from Truck Suvidha.
- A separate dataset with geographical data for analysis.





