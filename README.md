# nafsi-track1-submission--track-1
# NourishNet Data Pipeline

## Overview

This repository contains the data pipeline for **NourishNet**, a food access and resource discovery project created for the NAFSI Track 1 submission.

The pipeline collects and processes food assistance/resource data from multiple sources, including Google Sheets, public food resource websites, 211 Maryland search results, and OpenStreetMap. The final output is a structured JSON file that can be used by a frontend application to display food banks, food pantries, soup kitchens, and related community resources.

## Features

* Loads source data from Google Sheets
* Extracts resource links from spreadsheet tabs
* Scrapes public food assistance websites
* Searches food pantry resources from 211 Maryland
* Uses OpenStreetMap Overpass API to collect food bank and soup kitchen locations
* Cleans raw location data into structured JSON format
* Generates downloadable JSON outputs for frontend integration

## Data Sources

The pipeline uses publicly available sources such as:

* Google Sheets
* Feeding America
* Maryland Open Data
* DC Open Data
* Virginia Open Data
* Capital Area Food Bank
* Maryland Food Bank
* 211 Maryland
* OpenStreetMap Overpass API

## Output Files

The notebook generates JSON files such as:

* `data.json` — scraped website text and metadata
* `food_data.json` — food pantry data from 211 Maryland
* `food_locations.json` — cleaned food resource locations from OpenStreetMap

## Technologies Used

* Python
* Pandas
* Requests
* BeautifulSoup
* JSON
* OpenStreetMap Overpass API
* Google Colab / Jupyter Notebook

## How to Run

1. Clone this repository:

```bash
git clone https://github.com/YOUR_USERNAME/nafsi-track1-submission.git
cd nafsi-track1-submission
```

2. Install dependencies:

```bash
pip install pandas requests beautifulsoup4
```

3. Open the notebook:

```bash
jupyter notebook NourishNet_Data_Pipeline.ipynb
```

4. Run all cells from top to bottom.

5. The final output file will be:

```bash
food_locations.json
```

This file can be used in the NourishNet frontend application.

## Project Workflow

1. Load food resource data from Google Sheets
2. Identify useful URLs from the dataset
3. Scrape food assistance websites
4. Query food pantry information
5. Collect location data using OpenStreetMap
6. Clean and structure the data
7. Export final JSON files

## Team

* Saranya Roy
* Ayush 

## Repository Purpose

This repository documents the backend data collection and preprocessing work for the NourishNet project. It helps convert scattered public food assistance information into structured, usable data for an application.
