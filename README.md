# Sapphire IQ — Supermarket Sales Analysis

[![Project](https://img.shields.io/badge/Project-Data%20Analytics-2563eb)](https://github.com/Kxm-315006/Sapphire-IQ-Supermarket-Sales-Analysis)
[![Tool](https://img.shields.io/badge/Tool-Microsoft%20Excel-217346)](https://www.microsoft.com/microsoft-365/excel)
[![Status](https://img.shields.io/badge/Status-Completed-16a34a)](https://github.com/Kxm-315006/Sapphire-IQ-Supermarket-Sales-Analysis)

**Sapphire IQ Data Analytics Internship Project**

A supermarket sales analysis project built from the supplied project brief and grocery sales workbook. The project includes a cleaned analytical dataset, descriptive analysis, supporting documentation, and an interactive Excel dashboard.

## Project objectives

- Evaluate overall sales performance using total, average, median, minimum, and maximum sales.
- Compare sales across product categories, outlet types, outlet location tiers, and fat-content groups.
- Examine item visibility in relation to sales.
- Summarize data quality and statistical patterns.
- Present key findings in an interactive Excel dashboard.

## Main deliverable

**[Open the Excel dashboard](output/Sapphire_IQ_Supermarket_Sales_Analysis.xlsx)**

The workbook contains four sheets:

| Sheet | Contents |
|---|---|
| Dashboard | KPI cards, dropdown filters, category and outlet charts, fat-content comparison, and visibility-versus-sales scatter plot |
| Cleaned Data | All 8,523 source records, original fields, and a separate standardized fat-content field |
| Analysis | Category, outlet, location, and fat-content summaries plus descriptive statistics |
| Read Me | Dashboard guidance and data-quality notes |

### Dashboard filters

Use the dropdowns on the Dashboard sheet to filter by:
- Outlet Type
- Location Tier
- Fat Content

The KPI cards and category sales chart respond to the selected filters. The outlet and fat-content comparison charts use the relevant filters for their comparisons.

## Dataset overview

- **Records:** 8,523
- **Original fields:** 12
- **Missing values:** 1,463 in `Item Weight`
- **Exact duplicate rows:** None detected
- **Source currency:** Not specified in the supplied materials

The original dataset is preserved in `data/source/`. Missing item weights are left blank; no imputation was applied. Fat-content labels are standardized in a separate analytical field, while the original values remain unchanged.

## Key findings

| Measure | Result |
|---|---:|
| Total sales | 1,201,681.49 |
| Average sales per record | 140.99 |
| Median sales | 143.01 |
| Average item visibility | 0.0661 |
| Top four category share of sales | 50.60% |
| Visibility-sales Pearson correlation | -0.0013 |

Additional findings:
- **Highest-sales category:** Fruits and Vegetables (178,124.08).
- **Lowest-sales category:** Seafood (9,077.87).
- **Highest-sales outlet type:** Supermarket Type1 (787,549.89).

These are descriptive results based on the supplied records. Correlation does not establish causation, and outlet sales totals are not normalized for the number of records per outlet.

## Repository contents

```text
Sapphire-IQ-Supermarket-Sales-Analysis/
├── data/
│   └── source/
│       ├── BlinkIT_Grocery_Raw_Data.xlsx
│       └── Sapphire_IQ_Project_Brief.pdf
├── docs/
│   ├── ANALYSIS_SUMMARY.md
│   ├── DATA_DICTIONARY.md
│   └── METHODOLOGY.md
├── output/
│   └── Sapphire_IQ_Supermarket_Sales_Analysis.xlsx
├── .gitignore
└── README.md
```

## Documentation

- [Analysis summary](docs/ANALYSIS_SUMMARY.md)
- [Data dictionary](docs/DATA_DICTIONARY.md)
- [Methodology](docs/METHODOLOGY.md)
- [Original project brief](data/source/Sapphire_IQ_Project_Brief.pdf)

## How to use the project

1. Download the Excel workbook from the `output/` folder.
2. Open it in Microsoft Excel (desktop Excel is recommended for full workbook compatibility).
3. Open the **Dashboard** sheet.
4. Choose values from the three dropdown filters to explore the results.
5. Review the **Analysis** and **Cleaned Data** sheets for supporting detail.

## Methodology at a glance

1. Reviewed the supplied project brief and source workbook.
2. Loaded all 8,523 records and retained the 12 original columns.
3. Checked missing values and exact duplicate rows.
4. Preserved missing item weights without imputation.
5. Standardized fat-content labels in an additional field.
6. Calculated descriptive statistics, category and outlet summaries, and Pearson correlation.
7. Built the Excel dashboard and documented interpretation limits.

See [Methodology](docs/METHODOLOGY.md) for details.

## Project limitations

- The supplied source does not identify a currency; sales are reported in source units.
- Missing `Item Weight` values were not imputed.
- Correlation is descriptive and should not be interpreted as evidence of causation.
- Sales totals are not adjusted for differences in outlet record counts.
- Dashboard behavior and formatting may vary in spreadsheet applications other than Microsoft Excel.

## Project status

**Completed —** analysis, documentation, Excel dashboard, and source materials are included in this repository.

---

*Prepared as a data analytics internship project using the supplied Sapphire IQ project materials.*
