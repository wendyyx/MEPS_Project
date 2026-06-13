# MEPS 2022: Self-Rated Health and Insurance Coverage

## Overview

This project examines whether individuals' subjective assessment of their own health status influences their probability of holding health insurance coverage, using data from the 2022 Medical Expenditure Panel Survey (MEPS).

## Research Question

Does self-rated health status affect insurance coverage?

## Data

- **Source**: Medical Expenditure Panel Survey (MEPS), Full Year Consolidated File, HC-243 (2022)
- **Sample**: Adults aged 18–64 (N = 12,469 after cleaning)

> Raw data files (`h243.dat`, `h243su.txt`) are not included in this repository due to file size.  
> Please download them from the AHRQ website and place them in `data/raw/`.

## Project Structure

```
MEPS_Project/
├── data/
│   ├── raw/                            # Raw MEPS files (not tracked by Git)
│   │   ├── h243.dat
│   │   └── h243su.txt
│   └── clean/                          # Cleaned analytic dataset (auto-generated)
│       └── meps_analytic.csv
├── outputs/                            # Figures and tables (auto-generated)
│   ├── fig1_coverage_by_health.png
│   ├── fig2_health_distribution.png
│   ├── table1_descriptive.csv
│   └── Table2_regression_results.xlsx
├── AAE718_Week4_Project4_Yuxin.py      # Main analysis script
├── .gitignore
└── README.md
```

## How to Run

1. Download `h243.dat` and `h243su.txt` from AHRQ and place in `data/raw/`
2. Open `AAE718_Week4_Project4_Yuxin.py` in Jupyter Notebook or run directly:

```bash
python AAE718_Week4_Project4_Yuxin.py
```

3. Outputs are saved automatically to `outputs/`