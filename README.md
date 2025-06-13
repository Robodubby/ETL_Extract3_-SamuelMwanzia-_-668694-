# PROJECT TITLE: ETL Extract Lab

- Samuel Mwanzia  
- Student ID 668694  
---

## Overview

This project demonstrates the concepts of **Full Extraction** and **Incremental Extraction** in the ETL (Extract, Transform, Load) process using synthetic sales data.

---

## 📁 Project Structure
ETL_Extract_SamuelMwanzia_668694/
- .gitignore # Excludes unnecessary files
- custom_data.csv # Synthetic sales dataset
- etl_extract.ipynb # Main Jupyter Notebook with code 
- last_extraction.txt # Tracks the last extraction timestamp
- README.md # Project summary and instructions 

  Downloads/
- transformed_full.csv       # Transformed full data
- transformed_incremental.csv # Transformed incremental data
  
# SCREENSHOTS/
- FullExtraction.png
- GeneratedData.png
- IncrementalExtractions.png

## 🛠️ Tools Used

- Python
- pandas
- Jupyter Notebook

## How to Reproduce

1. Clone or download the project.
2. Open `etl_extract.ipynb` in Jupyter Notebook.
3. Run the cells in order:
   - Section 1: Full Extraction (loads and displays all data)
   - Section 2: Incremental Extraction (loads only new/updated data)
4. The `last_extraction.txt` file is automatically updated with the most recent timestamp after each incremental extraction.


## Dataset

A synthetic dataset (`custom_data.csv`) was generated using Python. It simulates 60 days of customer sales data with randomized timestamps and values

## Screenshot of Ouputs
Find Attached to the screenshots folder.

## SECTION AND EXPLANATIONS in ETL.ipynb (File with codes).

Section 1: Full Extraction
We loaded the entire dataset (custom_data.csv) and displayed the first few rows to get a general sense of the data's structure and size.

Section 2: Incremental Extraction
We simulated an incremental extraction by only selecting records with a last_updated timestamp after a saved date (last_extraction.txt). This allows future data updates to be processed without reloading the full dataset.

Section 3: Transform Full Data
We applied three transformation techniques on the full dataset:

Cleaning: Removed duplicate rows.

Enrichment: Added a total_price column by multiplying quantity and unit_price.

Structural: Converted the date column to a proper datetime format.

The transformed result was saved to transformed_full.csv.

Section 4: Transform Incremental Data
Similar transformations were applied to the incremental data:

Filled missing columns (quantity, unit_price) with simulated values.

Calculated total_price and standardized date format.

Saved as transformed_incremental.csv.

Section 5: Output and Export
Both transformed datasets were stored in a /Download/ folder:

transformed_full.csv

transformed_incremental.csv

These files are clean, enriched, and ready for analysis.



