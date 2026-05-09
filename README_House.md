# London housing market analysis 🏠

Exploratory data analysis on **13,549 records** of London housing data spanning **25 years (1995–2020)**, covering average prices, sales volume, and crime rates across 45 areas.

---

## Project overview

This project analyses the London housing dataset to answer key questions:
- How have average house prices changed across London from 1995 to 2020?
- Which areas have the highest and lowest average property prices?
- What is the relationship between crime rates and house prices?
- How did the 2008 financial crisis impact the housing market?
- Which years saw the highest volume of houses sold?

---

## Dataset

| Property | Detail |
|---|---|
| Source | London Housing Dataset (Kaggle) |
| Rows | 13,549 records |
| Columns | 6 (date, area, average_price, code, houses_sold, no_of_crimes) |
| Coverage | 45 London areas, January 1995 – January 2020 |
| Time span | 25 years of monthly data |

---

## Tools & libraries

![Python](https://img.shields.io/badge/Python-3.10-blue)
![Pandas](https://img.shields.io/badge/Pandas-2.0-green)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.7-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-0.12-teal)
![NumPy](https://img.shields.io/badge/NumPy-1.24-yellow)

---

## Key findings

- **House prices rose sharply** from ~£91K in 1995 to over £400K by 2020 across London on average
- **City of London and Kensington** consistently hold the highest average prices throughout the dataset
- **The 2008 financial crisis** caused a visible dip in both prices and houses sold, recovering by 2012
- **Areas with higher crime rates** tend to show lower average house prices — a negative correlation exists
- **Houses sold peaked in the early 2000s** and have been declining since, despite rising prices
- **Filtering to areas above £100K** average removes outlier records and gives a cleaner picture of the mainstream market

---

## Data cleaning steps

- Converted `date` column from string to datetime format
- Extracted `year` as a separate column for time-based grouping
- Filtered records where `average_price > 100,000` to remove outlier/incomplete entries
- Handled missing values in `houses_sold` and `no_of_crimes` columns

---

## Project structure

```
london-housing-analysis/
│
├── House_Analysis.ipynb          # Main analysis notebook
├── HouseData.csv                 # Dataset (source: Kaggle)
├── requirements.txt              # Python dependencies
└── README.md                     # This file
```

---

## How to run

1. Clone this repository
   ```bash
   git clone https://github.com/ManasDhotre/london-housing-analysis.git
   cd london-housing-analysis
   ```

2. Install dependencies
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter and open the notebook
   ```bash
   jupyter notebook House_Analysis.ipynb
   ```

---

## Author

**Manas Dhotre**
Aspiring Data Scientist | Python · Pandas · Data Analysis
📍 Pune, India

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue)](https://www.linkedin.com/in/manas-dhotre)
[![GitHub](https://img.shields.io/badge/GitHub-Follow-black)](https://github.com/ManasDhotre)

---

## Acknowledgements

Dataset sourced from [Kaggle – London Housing Data](https://www.kaggle.com/datasets/justinas/housing-in-london)
