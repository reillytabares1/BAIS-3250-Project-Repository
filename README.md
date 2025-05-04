# Data Wrangling Project Template

This template serves as a starting point for our data wrangling project. It includes a folder structure, sample data dictionary, notebook, and links to our datasets.

## Folder Structure

| Folder | Purpose |
|--------|---------|
| `data/raw/` | Original, unmodified data files |
| `data/processed/` | Cleaned datasets used in analysis |
| `notebooks/` | Jupyter notebooks for wrangling |
| `data_dictionary/` | Data dictionary in CSV format |

##  Table of Contents

1. [Overview](#overview)
2. [Folder Structure](#folder-structure)
3. [Notebook](#notebook)
4. [Data Sources](#data-sources)
5. [Data Dictionary](#data-dictionary)

##  Overview

This repository investigates the relationship between crime and unemployment in Los Angeles using public datasets. It’s intended as a reusable template and act as a project starting point.

##  Notebook

`notebooks/data_wrangling_los_angeles.ipynb`: Contains data cleaning, merging, and initial analysis steps.

##  Data Sources

- LAPD Arrest Data: (https://catalog.data.gov/dataset/arrest-data-from-2020-to-present) (csv file uploaded under raw)
- Unemployment Census Tracts: (https://data.lacounty.gov/datasets/lacounty::unemployment-census-tract/explore?location=33.733638%2C-118.298767%2C6.48&showTable=true)

##  Data Dictionary

| Column Name            | Type     | Source              | Description                                                                 |
|------------------------|----------|---------------------|-----------------------------------------------------------------------------|
| Report ID              | Numeric  | la_crime2023        | Unique crime ID                                                             |
| Arrest Date            | Date     | la_crime2023        | Date of crime                                                               |
| Area ID                | Numeric  | la_crime2023        | Unique ID of Community                                                      |
| Community              | Text     | both                | Neighborhood where the crime was committed                                  |
| Age                    | Numeric  | la_crime2023        | Age of perpetrator                                                          |
| Sex Code               | Text     | la_crime2023        | Sex of perpetrator                                                          |
| Charge Group Description | Text   | la_crime2023        | Group of charge (e.g., homicide, burglary)                                  |
| Charge Description     | Text     | la_crime2023        | Specifics of charge (e.g., Robbery → Carjacking)                            |
| Address                | Text     | la_crime2023        | Street address where the crime occurred                                     |
| Percent Unemployed     | Numeric  | unemployed_grouped  | Percent of population in the community that is unemployed                   |
| Supervisor District    | Numeric  | unemployed_grouped  | District that the community is in (used for grouping, not analysis)         |



