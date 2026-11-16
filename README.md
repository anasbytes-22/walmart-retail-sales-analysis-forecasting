# Walmart Retail Sales Analysis & Forecasting

Exploratory analysis and baseline sales forecasting on the Walmart M5 dataset using Python and Pandas.

## Objectives

- Understand the structure of the Walmart M5 sales data
- Clean and prepare the data for analysis
- Identify sales and pricing patterns through exploratory analysis
- Build and evaluate a simple baseline forecast of Walmart's total daily sales

## Dataset

This project uses the **M5 Forecasting - Accuracy** dataset from Kaggle:
https://www.kaggle.com/competitions/m5-forecasting-accuracy

Files used: `calendar.csv`, `sales_train_evaluation.csv`, `sales_train_validation.csv`, `sample_submission.csv`, `sell_prices.csv`.

The raw CSV files are not included in this repository because of their size. See `data/raw/README.md` for where to place them.

## Tools Used

Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook (VS Code)

## Project Structure

```
├── data/
│   ├── processed/
│   └── raw/            # place Kaggle CSV files here (not included)
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_Exploratory_data_analysis.ipynb
│   └── 04_sales_forecasting.ipynb
└── README.md
```

## Notebooks

1. **01_data_understanding**: loads each dataset, checks shapes and columns, and explains what each file represents.
2. **02_data_cleaning**: prepares the data for analysis. [FILL: 2-4 main cleaning steps]
3. **03_Exploratory_data_analysis**: explores sales and price patterns using descriptive statistics and Matplotlib visualizations.
4. **04_sales_forecasting**: builds and evaluates a simple baseline forecast of total daily sales.

## Key Findings

- The selling price distribution is skewed: the mean (about 4.41) is higher than the median (about 3.47), meaning a smaller number of higher-priced items pull the average up.
- [FILL: sales finding 1]
- [FILL: sales finding 2]
- [FILL: sales finding 3]

## Forecasting Methodology and Results

**Goal:** forecast Walmart's total daily sales using historical sales data.

**Method:** [FILL: how the baseline forecast was calculated]

**Evaluation:** the forecast was tested on a 28-day period [FILL: test dates] and measured with Mean Absolute Error (MAE).

| Metric | Result |
|---|---|
| Baseline forecast | about 34,342 units per day |
| Mean Absolute Error (28 test days) | 9,650.01 units per day |

The average error is roughly 28% of the forecast level, so this baseline is a starting point for comparison, not a highly accurate model.

## Limitations

- The forecast is a simple baseline, and its error is large relative to daily sales.
- It forecasts total daily sales only, not individual products or stores.
- No advanced forecasting models were tried in this project.

## How to Reproduce

1. Clone this repository.
2. Download the M5 CSV files from Kaggle and place them in `data/raw/`.
3. Install the libraries: `pip install -r requirements.txt`
4. Open the notebooks in VS Code or JupyterLab and run them in order, from 01 to 04.
