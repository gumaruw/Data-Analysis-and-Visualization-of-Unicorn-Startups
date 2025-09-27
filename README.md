# Unicorn Companies Missing Data Handling

This project was completed as part of my scholarship in the Data Science program at the Artificial Intelligence and Technology Academy. It was undertaken within the scope of the "Go Beyond the Numbers: Translate Data into Insights" chapter of the Google Advanced Data Analytics course.

## Overview

This project involves data analysis with a focus on handling missing data within a dataset related to unicorn companies, including their funding, valuation, and geographic distribution. The primary objectives were to:

- Detect and handle missing data effectively.
- Visualize key insights, such as the highest valued countries and the sectors that attract investors.
- Understand the impact of missing data handling techniques on the analysis results.

## Dataset

- **Name:** `Unicorn_Companies.csv`
- **Source:** Kaggle
- **Rows:** 1,074 unicorn companies
- **Columns:** 10 (including company name, valuation, funding, industry, investors, etc.)

### Key Columns

- `Company`: Name of the unicorn company  
- `Valuation`: Company valuation (in billions)  
- `Date Joined`: Date the company became a unicorn  
- `Industry`: Business industry  
- `Funding`: Total funding raised  
- `Year Founded`: Year the company was founded  
- `Select Investors`: Top investors  
- `Country/Region`, `Continent`, `City`: Geolocation details  

## Key Steps

- **Missing Data Detection**  
  Missing data was identified using the `isna()` function, and rows containing at least one missing value were filtered using `any(axis=1)`.

- **Handling Missing Data**  
  - Dropped rows with minimal missing values.  
  - Imputed missing values in certain columns (e.g., Funding, Select Investors) with default values or categories.  
  - Explored alternative imputation methods such as mean/mode or predictive models.

- **Data Visualization**  
  - Valuation of unicorns by country using circle charts where size represents total valuation.  
  - Analyzed highest performing regions, focusing on Europe and the Middle East.

- **Analysis Results**  
  - Identified 17 companies meeting investor criteria.  
  - Highest total valuations observed in the USA, China, India, the UK, and Germany.

## Example Insights

- Europe and the Middle East show high activity in terms of unicorns and investor interest.  
- Row deletion for missing data resulted in less data loss than column deletion.  
- Imputed values were mostly reasonable but may require manual verification for accuracy.

## How to Run

1. Clone the repository  
2. Open the Jupyter Notebook file  
3. Ensure `Unicorn_Companies.csv` is in the same directory  
4. Run the notebook step-by-step

```bash
git clone https://github.com/gumaruw/Unicorn-Companies-Missing-Data-Handling.git
cd Unicorn-Companies-Missing-Data-Handling
jupyter notebook

```
