# Methodology

1. Used the supplied Sapphire IQ project brief and the supplied Excel dataset as the only project sources.
2. Loaded all 8,523 rows and retained all 12 original columns.
3. Checked exact duplicate rows and missing values.
4. Preserved missing `Item Weight` values as blanks; no imputation was performed.
5. Added a separate `Fat Content (Clean)` field to standardize `LF` and `low fat` as `Low Fat`, and `reg` as `Regular`. The original field remains unchanged.
6. Calculated total, average, median, minimum, maximum, sample standard deviation, sample variance, quartiles, IQR fences, and IQR outlier count.
7. Compared sales by product category, outlet type, location tier, and fat content.
8. Calculated Pearson correlation between Item Visibility and Sales. This is descriptive and not causal.

## Dashboard interaction
The Dashboard sheet includes dropdown filters for Outlet Type, Location Tier, and Fat Content. The KPI cards and category sales chart respond to the selected filters. Outlet type sales responds to location and fat-content filters. The Low Fat vs Regular outlet comparison responds to outlet type and location filters.
