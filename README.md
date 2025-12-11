# Singapore HDB Resale Price Analysis 🇸🇬

This project is an exploratory data analysis (EDA) website built with **R** and **Quarto**. [cite_start]It investigates the trends, drivers, and spatial patterns of public housing (HDB) resale prices in Singapore, contrasting its unique 99-year leasehold system with market-driven models like New York City[cite: 1, 6, 12].

## 📊 Project Overview

[cite_start]Approximately 80% of Singaporeans live in HDB flats[cite: 2, 8]. [cite_start]This project aims to demystify the factors influencing resale prices—specifically location, flat type, storey height, and lease duration[cite: 5, 14].

**Key Analyses:**
* [cite_start]**Macro Trends:** Evolution of median prices over the last 15 years, including the impact of COVID-19 and cooling measures[cite: 63, 64].
* [cite_start]**Lease Decay:** Analysis of the non-linear relationship between remaining lease and price, highlighting the "U-shaped" resilience of large flats in mature estates[cite: 93].
* [cite_start]**The "Million-Dollar" Phenomenon:** Spatial mapping of luxury HDB transactions to determine if high prices are driven by size or location[cite: 104, 111].
* [cite_start]**Vertical Equity:** Quantifying the price premium commanded by higher floor levels[cite: 119].

## 📂 Data Sources

[cite_start]The analysis utilizes two official datasets from [Data.gov.sg](https://data.gov.sg/)[cite: 20]:
1.  [cite_start]**Median Resale Prices:** Aggregated data by town and flat type to analyze broad market shifts[cite: 24].
2.  [cite_start]**Transaction-Level Data (2017–Present):** Granular data including floor area, storey height, and remaining lease for micro-level analysis[cite: 25, 26].

## 🛠️ Tech Stack

* **Framework:** [Quarto](https://quarto.org/) (Website generation)
* **Language:** R
* **Key Libraries:**
    * [cite_start]`tidyverse` (Data manipulation & visualization) [cite: 33]
    * [cite_start]`sf` (Geospatial mapping of planning areas) [cite: 33]
    * [cite_start]`naniar` (Missing data analysis) [cite: 33]
    * [cite_start]`mgcv` (Generalized Additive Models for lease curves) [cite: 82]

## 🚀 How to Run

1.  Clone this repository.
2.  Open the project in RStudio.
3.  Ensure the `datasets/` folder contains the required CSV files.
4.  Render the website via the terminal:
    ```bash
    quarto render
    ```
5.  The generated site will be available in the `_site/` directory.
