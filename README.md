# DC Region Capital Flows Analysis

An exploratory data analysis examining the relationship between capital investment, poverty rates, and racial demographics across counties in the Washington D.C. region.

**[Read the rendered report](https://sys9317.github.io/dc-capital-flows-analysis/)** &nbsp;·&nbsp; source in [`dc_capital_flows_analysis.qmd`](dc_capital_flows_analysis.qmd) (Quarto). Rebuild with `quarto render dc_capital_flows_analysis.qmd`.

---

## Overview

This project uses publicly available data from the Urban Data Catalog to investigate whether capital investment is equitably distributed across the DC region. Specifically, it explores:

- Whether county population size correlates with local poverty rates
- How aggregate investment per household varies across racial demographic categories
- Geographic patterns in poverty across the contiguous U.S.

## Key Findings

- **Population & Poverty:** A negative linear trend suggests that larger, more urbanized counties tend to have lower poverty rates — though population alone is not a strong standalone predictor.
- **Race & Investment:** Median investment per household varies meaningfully across racial demographic categories, pointing to potential structural disparities in capital distribution.
- **Geographic Patterns:** Spatial analysis is planned as an extension once county geometries are joined via FIPS codes.

## Project Structure

```
dc-capital-flows-analysis/
├── dc_capital_flows_analysis.qmd   # Main analysis (Quarto)
├── data/
│   └── DC Region Capital Flows Feature Data - Catalog Version.xlsx   # raw data (committed, ~45 KB)
├── LICENSE
└── README.md
```

Run `quarto render` to produce `dc_capital_flows_analysis.html`.

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/sys9317/dc-capital-flows-analysis.git
cd dc-capital-flows-analysis
```

### 2. Data

The raw data file is included in `data/` (public, ~45 KB).

**Source:** [DC Region Capital Flows Feature Data (Urban Data Catalog, 2023)](https://urban-data-catalog.s3.amazonaws.com/drupal-root-live/2023/01/25/DC%20Region%20Capital%20Flows%20Feature%20Data%20-%20Catalog%20Version.xlsx)

### 3. Render the report

```bash
quarto render dc_capital_flows_analysis.qmd
```

## Tools & Packages

- **Language:** R
- **Report:** Quarto (`.qmd`)
- **Core packages:** `tidyverse`, `readxl`, `ggplot2`, `tigris`, `sf`, `scales`

## Data Source

Urban Institute — Urban Data Catalog (2023).
*DC Region Capital Flows Feature Data.*
[https://urban-data-catalog.s3.amazonaws.com](https://urban-data-catalog.s3.amazonaws.com/drupal-root-live/2023/01/25/DC%20Region%20Capital%20Flows%20Feature%20Data%20-%20Catalog%20Version.xlsx)

---

*By Yosup Shin*
