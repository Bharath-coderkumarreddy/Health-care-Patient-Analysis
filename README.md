# Healthcare Patient Analysis

A data analytics project focused on preparing healthcare data and presenting it for exploration using **Python, Pandas, Jupyter Notebook, and Microsoft Power BI**.

## Project Overview

This project uses a healthcare dataset to inspect patient-related records, prepare the data for analysis, and support visual exploration through a Power BI report. The Python notebook documents the data preparation workflow, while the Power BI file provides a report interface for exploring the available data.

## Project Objectives

- Inspect the structure and quality of the healthcare dataset.
- Identify and handle selected missing values.
- Convert admission and discharge dates to appropriate date types.
- Prepare a cleaned dataset for further analysis.
- Use Power BI to explore the prepared healthcare data.

## Project Files

| File | Description |
|---|---|
| `HealthcareDataset1.csv` | Source healthcare dataset |
| `CAPSTONE PROJECT(1).ipynb` | Jupyter Notebook for data inspection and preparation |
| `CAPSTONE PROJECT (1)(1).pbix` | Power BI report file |

*File names in this table should match the names used in your repository. Rename them here if you choose different names when uploading.*

## Dataset Description

The source CSV contains **1,000 records and 11 columns**.

| Column | Description |
|---|---|
| `PatientID` | Patient identifier |
| `PatientName` | Patient name |
| `Age` | Patient age |
| `Gender` | Gender category recorded in the dataset |
| `BloodType` | Patient blood type |
| `Diagnosis` | Recorded diagnosis |
| `Treatment` | Treatment category |
| `AdmissionDate` | Date of admission |
| `DischargeDate` | Date of discharge |
| `TotalBill` | Recorded bill amount |
| `Full Prescription Details` | Prescription details recorded for the patient |

## Tools and Technologies

- **Python** — data preparation
- **Pandas** — data loading, inspection, and transformation
- **Jupyter Notebook** — interactive analysis workflow
- **Microsoft Power BI** — data visualization and report exploration
- **CSV** — dataset storage and exchange

## Data Preparation

The notebook includes the following preparation steps:

1. Load the CSV data into a Pandas DataFrame.
2. Inspect sample records, data types, and descriptive statistics.
3. Check for missing values in the patient-name field and remove records where the patient name is missing.
4. Fill missing values in `TotalBill` using the fixed value `10038.866970`.
5. Convert `AdmissionDate` and `DischargeDate` to datetime types.
6. Export the prepared data to `Healthcare_Cleaned.csv`.

**Data-quality note:** The notebook uses a fixed value to fill missing bill amounts. This choice should be reviewed before interpreting billing results. Validate the imputation approach and check for remaining missing values, duplicates, invalid dates, and outliers as part of data quality assurance.

## Power BI Report

The `.pbix` file contains the Power BI report associated with this project. Open it in Power BI Desktop to review the report and explore the visuals available in the file. If prompted, update the data-source path to the location of your CSV or cleaned dataset and refresh the report.

## How to Run the Project

### 1. Requirements

Install Python and Jupyter Notebook, then install Pandas:

```bash
pip install pandas jupyter
```

### 2. Run the notebook

1. Download or clone the repository.
2. Place the source CSV in the project folder, or update the CSV path in the notebook.
3. Open the notebook in Jupyter Notebook or JupyterLab.
4. Run the cells in order.
5. Confirm that `Healthcare_Cleaned.csv` is created in the expected location.

### 3. Open the Power BI report

1. Open the `.pbix` file in Microsoft Power BI Desktop.
2. If necessary, point the report to the correct data file.
3. Refresh the data and review the report visuals.

## Limitations

- The dataset has not been independently verified for accuracy or representativeness.
- The method used to fill missing billing values may affect analysis results.
- This project is intended for data analytics practice and should not be used to make medical diagnoses or treatment decisions.

## Data Privacy

The dataset includes patient names and prescription details. Before publishing this project publicly, ensure you have permission to share the data and remove or anonymize personally identifiable or sensitive information.

## Author

**Mukka Bharath Kumar Reddy**

*Data Analytics Project Developer*
