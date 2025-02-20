# Web Scraping Load Details from Truck Suvidha

## Overview

This project focuses on web scraping a table containing load details from the Truck Suvidha website. The script extracts information such as source city, destination city, distance, weight, scheduled date, material, truck type, and other relevant details.

## Requirements

- Python 3.x
- Required libraries:
  - `requests`
  - `BeautifulSoup`
  - `pandas`

## Installation

Ensure you have the necessary libraries installed by running:

```sh
pip install requests beautifulsoup4 pandas
```

## Usage

1. Modify the script to include the correct URL of the Truck Suvidha load details page.
2. Run the script using:

```sh
python TruckSuvidha(websraping).ipynb
```

3. The extracted data will be saved as a CSV file (`TruckSuvidha_Loaddata.csv`).

## Output

- Extracted table data will be stored in a Pandas DataFrame.
- The cleaned data will be saved in `TruckSuvidha_Loaddata.csv`.



