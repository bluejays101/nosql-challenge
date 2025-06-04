
# NoSQL Challenge: UK Food Standards Agency Ratings

## Overview

This project demonstrates the use of MongoDB and PyMongo to import, clean, and analyze the UK Food Standards Agency's food establishments dataset. It is designed as a practical NoSQL data engineering and analytics exercise, with reproducible steps in Jupyter notebooks.

## Features

- Import large JSON datasets into MongoDB using `mongoimport`
- Inspect, insert, update, and clean data using PyMongo
- Perform exploratory data analysis with custom queries and aggregation pipelines
- Convert and analyze MongoDB results using pandas DataFrames

## File Structure

```
.
├── NoSQL_setup_starter.ipynb         # Notebook for data import, setup, and cleaning
├── NoSQL_analysis_starter.ipynb      # Notebook for exploratory analysis and reporting
├── establishments.json               # Raw data file for import
└── README.md
```

## Technologies

- MongoDB Community Server
- PyMongo
- Python 3.x (Jupyter Notebook)
- pandas

## Getting Started

1. **Import Data**  
   Open terminal or PowerShell in your project directory and run:
   ```bash
   mongoimport --type json -d uk_food -c establishments --drop --jsonArray establishments.json
   ```

2. **Start MongoDB**  
   Ensure the MongoDB service is running on your computer.

3. **Open Jupyter Notebooks**  
   Run the notebooks in order:
   - `NoSQL_setup_starter.ipynb`: Performs all database setup and data cleaning tasks.
   - `NoSQL_analysis_starter.ipynb`: Contains all exploratory queries and analysis.

## Usage

- Make sure `establishments.json` is present in the project folder.
- Follow the step-by-step instructions within each notebook cell.
- All queries use PyMongo and results are explored using pandas.
---
