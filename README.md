# econ5200-lab02-deflation
# Index Integrity — Deflation, Substitution Bias & Goodhart

## Objective

In this lab, I learned how to identify errors in economic data calculations, compare price indexes, and understand how performance targets can affect the quality of results.

## Methodology

- I identified and fixed four bugs in a deflation function, including an error that reported values in 1982–84 dollars instead of 2020 dollars.
- I compared CPI-U and C-CPI-U to measure upper-level substitution bias.
- I calculated their average annual inflation rates and compared the difference in percentage points with the difference in index points.
- I studied Goodhart's Law by examining the relationship between DAU/MAU and time per session during two different phases.
- I created `deflation_utils.py` with a `deflate_series()` function and tested it.
- I built an interactive monitor to compare price indexes, adjust the correlation window, and identify negative correlations.

## Key Findings

The average annual inflation rate was **2.63%** for CPI-U and **2.36%** for C-CPI-U. The difference was **0.27 percentage points per year**.

The index-point gap was **0.50 points per year**. This is different from the inflation-rate gap because index points measure changes in index levels, while percentage points compare annual growth rates.

The correlation between DAU/MAU and time per session changed from **+0.93** in the organic phase to **−0.96** in the gaming phase.

This change showed me that improving one performance metric does not always mean the overall result is better.

Overall, this lab taught me why checking calculations, understanding measurement methods, and monitoring multiple indicators are important in data analysis.
