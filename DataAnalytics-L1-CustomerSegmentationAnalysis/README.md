# Customer Segmentation Analysis

**Oasis Infobyte Data Analytics Internship — Level 1, Task 2**

This project segments e-commerce customers from the Online Retail dataset using Recency, Frequency, and Monetary (RFM) analysis and K-Means clustering. It turns transaction-level data into customer groups that can support targeted marketing and retention decisions.

## Objectives

- Clean retail transaction data and retain valid customer purchases.
- Build customer-level Recency, Frequency, and Monetary features.
- Select a suitable number of clusters with the elbow method.
- Group customers with K-Means and interpret the resulting segments.
- Export reusable CSV results and visualisations.

## Project structure

```text
DataAnalytics-L1-CustomerSegmentationAnalysis/
├── data/
│   └── Online Retail.xlsx
├── notebook/
│   └── customer_segmentation.ipynb
├── outputs/
│   ├── customer_segments.csv
│   ├── cluster_profile.csv
│   ├── elbow_method.png
│   ├── cluster_recency_frequency.png
│   ├── cluster_frequency_monetary.png
│   └── customers_per_segment.png
├── requirements.txt
└── README.md
```

## Requirements

- Python 3.11 to 3.14
- Internet access the first time dependencies are installed

The dataset is included in `data/`, so no additional download is required.

## Run the project from a ZIP download

1. Download and extract the repository ZIP.
2. Open PowerShell, Command Prompt, or a terminal in the extracted repository folder.
3. Create and activate a virtual environment.

   **Windows PowerShell**

   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```

   **Windows Command Prompt**

   ```bat
   python -m venv .venv
   .venv\Scripts\activate.bat
   ```

   **macOS / Linux**

   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

4. Install the required packages from the project folder.

   ```bash
   pip install -r requirements.txt
   ```

5. Start Jupyter **from the `notebook` folder**. This is required because the notebook reads `../data/Online Retail.xlsx` and writes to `../outputs/`.

   ```bash
   cd notebook
   jupyter lab
   ```

6. Open `customer_segmentation.ipynb` and choose **Run All Cells**.

The exported charts and CSV files will be available in the `outputs/` folder when execution finishes.

## Methodology

1. Remove records with no customer ID, duplicates, cancelled invoices, and invalid quantities or prices.
2. Calculate RFM metrics for each customer.
3. Apply `log1p` transformation and standard scaling to reduce skew and align feature scales.
4. Use the elbow method to select four clusters.
5. Train K-Means with a fixed random state (`42`) for reproducible results.
6. Profile and label the resulting customer groups.

## Outputs

| File | Description |
| --- | --- |
| `customer_segments.csv` | Customer-level RFM values, cluster number, and segment label. |
| `cluster_profile.csv` | Average RFM metrics and customer counts by cluster. |
| `elbow_method.png` | Inertia plot used to select the number of clusters. |
| `cluster_recency_frequency.png` | Recency versus frequency cluster visualisation. |
| `cluster_frequency_monetary.png` | Frequency versus monetary-value cluster visualisation. |
| `customers_per_segment.png` | Number of customers in each final segment. |

## Key insights

The analysis identifies four groups: **Champions**, **Loyal Customers**, **New / Potential Customers**, and **At Risk** customers. These groups can inform loyalty programmes, personalised offers, onboarding campaigns, and win-back initiatives.

## Troubleshooting

- **`FileNotFoundError` for `Online Retail.xlsx`:** start Jupyter from `notebook/`, not the repository root.
- **`python` is not recognised:** install Python 3.11–3.14 and select “Add Python to PATH” during installation.
- **PowerShell activation is blocked:** run `Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`, then activate `.venv` again.

## Author

Vamshi Kodi
