# DC Region Capital Flows Analysis

An exploratory data analysis examining the relationship between capital investment, poverty rates, and racial demographics across counties in the Washington D.C. region.

📊 **[View the full analysis report](https://github.com/sys9317/dc-capital-flows-analysis)** 
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
dc-capital-flows/
├── dc_capital_flows_analysis.qmd   # Main analysis (Quarto)
├── dc_capital_flows_analysis.html  # Rendered report
├── data/
│   ├── README.md                   # Instructions to download the raw data
│   └── *.xlsx                      # Gitignored — see data/README.md
└── README.md
```

## Getting Started

### 1. Clone the repo

```bash
git clone https://github.com/yourusername/dc-capital-flows.git
cd dc-capital-flows
```

### 2. Download the data

The raw data file is not tracked in this repository. Download it from the Urban Data Catalog and place it in the `data/` folder:

**Source:** [DC Region Capital Flows Feature Data (Urban Data Catalog, 2023)](https://urban-data-catalog.s3.amazonaws.com/drupal-root-live/2023/01/25/DC%20Region%20Capital%20Flows%20Feature%20Data%20-%20Catalog%20Version.xlsx)

Save as:
```
data/DC Region Capital Flows Feature Data - Catalog Version.xlsx
```

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
