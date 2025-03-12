# Truck Suvidha Web Scraping Project

## Overview
This project automates the collection of load details from the **Truck Suvidha** website, enriches it with geographical data, and stores it periodically. The script extracts transportation data, adds timestamps, fetches latitude, longitude, and population of destination cities, and saves it in CSV files for further analysis.

## Features
- Scrapes load details from the Truck Suvidha website using `pandas.read_html()`.
- Appends data to a CSV file with timestamps for historical tracking.
- Uses `geopy` to fetch latitude, longitude, and population of destination cities.
- Runs automatically every **10 minutes for 1 hour** using `schedule`.
- Generates graphs based on collected data for analytical insights.

## Data Collection
- **Source Website:** Truck Suvidha
- **Scraping Duration:** February 20, 2025 – Present
- **Scraping Interval:** Every 10 minutes for 1 hour
- **Data Storage Format:** CSV

### **Primary Dataset Fields**
The scraped data includes the following columns:
1. **Source City** – The city where the shipment originates.
2. **Destination City** – The target location of the shipment.
3. **Distance** – The distance between source and destination (in km).
4. **Weight (MT)** – The weight of the shipment in metric tons.
5. **Schd. Date** – The scheduled date of transportation.
6. **Material** – The type of goods being transported.
7. **Truck Type** – The type of truck required for transportation.
8. **Posted By** – The user who posted the shipment request.
9. **Details** – Additional details about the shipment.
10. **Quotation** – The estimated transportation cost.

### **Supplementary Dataset**
A secondary dataset was created to include geolocation and demographic information for each destination city. It consists of:
1. **Destination City** – The target location of the shipment.
2. **Latitude** – The latitude coordinate of the city.
3. **Longitude** – The longitude coordinate of the city.
4. **Population** – The total population of the city.

## Requirements
- Python 3.x
- Required libraries:
  - `pandas`
  - `datetime`
  - `os`
  - `schedule`
  - `time`
  - `geopy`
  - `matplotlib`

## Installation
Ensure you have the necessary libraries installed by running:
```sh
pip install pandas schedule geopy matplotlib
```

## Usage
1. Run the script to start scraping and storing data:
```sh
python TruckSuvidha_Loaddata_Script_py.py
```
2. The extracted data will be saved as:
   - `trucksuvidha_data.csv`: Contains load details with timestamps.
   - `destination_data.csv`: Contains geographical details of destination cities.
3. Once data collection is complete, graphs will be automatically plotted for analysis.

## Output
- A continuously updating dataset of load details from Truck Suvidha.
- A separate dataset with geographical data for analysis.
- Graphs generated for visualization and insights.

## Future Enhancements
- Extend the scraping duration for long-term trend analysis.
- Implement a real-time dashboard for live tracking of truck data.
- Integrate with a mapping API for better visualization of routes.




