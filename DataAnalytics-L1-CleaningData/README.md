# Data Analytics L1 — Cleaning Data

A beginner-friendly data-cleaning project that turns a deliberately messy, synthetic crime-incidents dataset into a clean, analysis-ready CSV.

> **Note:** All records are synthetic and are provided only for learning and portfolio practice.

## What's included

```text
DataAnalytics-L1-CleaningData/
├── Data/
│   ├── crime_incidents_messy.csv      # Original dataset
│   └── readme.md                      # Dataset details and data dictionary
├── notebook/
│   ├── DataCleaning.ipynb             # Jupyter notebook
│   └── crime_incidents_cleaned.csv    # Cleaned output dataset
├── requirements.txt
└── README.md
```

## What you will practice

- Loading and inspecting CSV data with Pandas
- Finding missing values and duplicate records
- Standardising inconsistent text and categorical values
- Converting columns to suitable data types
- Detecting outliers and validating the cleaned result

## Run on any computer

1. Download this repository using **Code → Download ZIP**, then extract the ZIP.
2. Open a terminal in the extracted `DataAnalytics-L1-CleaningData` folder.
3. Create and activate a virtual environment (recommended):

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

   On macOS/Linux, use `source .venv/bin/activate` instead.

4. Install the required packages:

   ```powershell
   python -m pip install -r requirements.txt
   ```

5. Start Jupyter:

   ```powershell
   jupyter notebook
   ```

6. Open `notebook/DataCleaning.ipynb` and run the cells from top to bottom.

The notebook locates the input data relative to its own folder, so it works whether you open it through Jupyter or after extracting a GitHub ZIP.

## Data

The source dataset has intentional quality problems—such as missing data, duplicate rows, inconsistent spellings/capitalisation, mixed date formats, numeric values stored as text, and outliers. See [Data/readme.md](Data/readme.md) for the dataset description and column information.

## Requirements

- Python 3.10 or later
- The packages in `requirements.txt`

## License

The synthetic dataset is released under [CC0 1.0](https://creativecommons.org/publicdomain/zero/1.0/). The accompanying project materials may be used for learning and portfolio purposes.
