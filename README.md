# Big Data ETL Assignment

This project implements an ETL (Extract, Transform, Load) pipeline for a large cybersecurity dataset using Python's Pandas library and PostgreSQL database.

## Dataset
- Source: `cybersecurity_attack.csv` (3,068,095 records)
- Relevant to business scenario: Cybersecurity attack logs for security monitoring and analysis

## ETL Process
1. **Extract**: Load data from CSV file using Pandas
2. **Transform**: 
   - Remove columns with more than 60% null values
   - Fill remaining null values with 0
3. **Load**: Store transformed data in PostgreSQL database

## Database Schema
The data is stored in a PostgreSQL table named `cybersecurity_logs` with automatically inferred column types based on the data structure.

## Files
- `extract.ipynb`: Data extraction from CSV.
- `Transform.ipynb`: Data cleaning and transformation.
- `Load.ipynb`: Loading data into PostgreSQL.
- `Data/`: Directory containing source and intermediate data files.
- `screenshots/`: Directory containing project screenshots.

## Screenshots

### Loaded Database
![Loaded Database](screenshots/loaded_database.png)

### Database Schema
![Database Schema](screenshots/database_schema.png)

### ETL Process
![ETL Process](screenshots/etl_process.png) 
