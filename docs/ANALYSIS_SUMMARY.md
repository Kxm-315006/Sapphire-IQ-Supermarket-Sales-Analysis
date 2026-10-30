# Analysis Summary

## Dataset overview

The supplied workbook contains **8,523 product records** and 12 original fields. The analysis uses the supplied `Sales` field and does not assume a currency because none is specified in the source files.

## Overall sales performance

| Metric | Result |
|---|---:|
| Total sales | 1,201,681.49 |
| Average sales per record | 140.99 |
| Median sales | 143.01 |
| Minimum sales | 31.29 |
| Maximum sales | 266.89 |
| Average item visibility | 0.0661 |
| Sample standard deviation | 62.28 |
| Sample variance | 3,878.18 |

## Category and outlet comparison

The top four product categories by sales are:

| Category | Total sales |
|---|---:|
| Fruits and Vegetables | 178,124.08 |
| Snack Foods | 175,433.92 |
| Household | 135,976.53 |
| Frozen Foods | 118,558.88 |

Together, the four largest categories contribute **50.60%** of total sales. The highest-sales category is **Fruits and Vegetables**; the lowest-sales category is **Seafood**.

| Outlet type | Total sales |
|---|---:|
| Supermarket Type1 | 787,549.89 |
| Grocery Store | 151,939.15 |
| Supermarket Type2 | 131,477.78 |
| Supermarket Type3 | 130,714.67 |

The highest-sales outlet type is **Supermarket Type1**.

## Visibility and statistical patterns

- Pearson correlation between Item Visibility and Sales: **-0.0013** (virtually no linear relationship).
- Q1: **93.83**; Q3: **185.64**; IQR: **91.82**.
- IQR lower fence: **-43.90**; upper fence: **323.37**.
- Sales records outside the IQR fences: **0**.

## Data quality

- `Item Weight` contains **1,463** missing values; these remain blank.
- No exact duplicate rows were detected.
- Fat-content labels are standardized in a separate analytical field: `LF` and `low fat` → `Low Fat`; `reg` → `Regular`. Original source values are preserved.
- The category-by-outlet-type matrix and outlet-level Low Fat/Regular comparisons are included in the workbook's Analysis and Dashboard sheets.

## Interpretation cautions

These are descriptive findings. Correlation does not establish causation. Sales totals are not normalized for outlet record counts. The supplied source does not specify currency.
