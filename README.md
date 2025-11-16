# Leeds Crime Patterns: A Comparative Analysis of Student Areas

A data analysis group project to identify and quantify the unique crime profile of student-heavy wards in Leeds.



## Overview

This project analyses 12 months of street-level crime data from `data.police.uk`. After acquiring, cleaning, and filtering the data for the Leeds area, we performed a comprehensive exploratory data analysis (EDA), geospatial hotspot mapping, and a final comparative analysis.

The core finding is that **student residential areas have a unique and statistically significant "crime fingerprint"**, distinct from both the commercial city centre and other residential wards.

## Key Findings

1.  **The "City Centre Effect"**: The 'Little London & Woodhouse' ward (which contains the city centre) is a massive outlier, driven by commercial crimes like **Shoplifting (19.3%)**.
2.  **The "Student" Profile**: Student-heavy wards (like 'Headingley & Hyde Park') have the highest proportional rates of **Burglary (6.9%)** and **Vehicle Crime (11.2%)**, indicating a "vulnerable residential" profile.
3.  **The "Baseline" Profile**: All other wards are defined by a high baseline of **Violence and sexual offences (39.5%)**.
4.  **Seasonal Spikes**: Crime is not static. We identified a clear "October spike" in Anti-social behaviour, which aligns with the return of the university population.



## Project Objectives

* **Objective 1: Data Acquisition & Cleaning**: Acquire, merge, and clean 12 months of police data. Filtered for Leeds using a geospatial join with official ONS ward boundaries.
* **Objective 2: Exploratory Data Analysis (EDA)**: Conducted a "baseline" analysis of the entire city to understand crime frequency, seasonality (temporal trends), and outcomes.
* **Objective 3: Geospatial Analysis**: Generated choropleth (heatmap) maps to visually separate the hotspots for *total crime* versus *specific crimes* (e.g., ASB, Burglary, Shoplifting).
* **Objective 4: Comparative Analysis**: Quantified the "crime fingerprint" of different area types (City Centre vs. Student Residential vs. Other) to statistically prove our hypothesis.

## Data Sources

* **Crime Data**: Street-level crime data for West Yorkshire (12-month period) from [data.police.uk](https://data.police.uk/data/).
* **Geospatial Data**: Ward boundaries and lookup tables from the [ONS Open Geography Portal](https://geoportal.statistics.gov.uk/).

## How to Run This Project

This project is built as a single, reproducible pipeline.

### Prerequisites

* Python 3.9+
* The raw data files were downloaded from the sources above.

### Installation

1.  Clone this repository:
    ```bash
    git clone https://github.com/nilavans/leeds-crime-patterns.git
    cd leeds-crime-patterns
    ```
2.  Create a `data` folder and place the downloaded raw CSVs and shapefiles inside, as described in the `group_project.ipynb` script.
3.  Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

### Execution

Run the main analysis script from your terminal or execute the cells in the Jupyter Notebook


### Contributors
Nilavan Sritharan
Asjad Moiz Khan
Krithik Sharan Suresh Alagianayagi
Zhenny Marifatul Hasna
