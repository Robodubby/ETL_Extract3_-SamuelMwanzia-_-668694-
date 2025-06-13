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

---

## Dataset

A synthetic dataset (`custom_data.csv`) was generated using Python. It simulates 60 days of customer sales data with randomized timestamps and values

## Screenshot of Ouputs
Find Attached to the screenshots folder.

