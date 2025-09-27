# Unicorn Companies Missing Data Handling

This project was completed as part of my scholarship in the Data Science program at the Artificial Intelligence and Technology Academy. Focuses on analyzing unicorn company data with an emphasis on handling missing values in funding, valuation, and geographic information.

## Overview
 
- Detect and handle missing data efficiently  
- Visualize key insights, such as top-valued countries and investor-attractive sectors  
- Assess the impact of missing data handling on analysis

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

- **Missing Data Detection:** Used `isna()` and filtered rows with `any(axis=1)`  
- **Handling Missing Data:** Dropped minimal missing rows, imputed others, explored mean/mode or predictive imputation  
- **Data Visualization:** Valuation by country (circle charts), analyzed top regions (Europe, Middle East)  
- **Analysis Results:** 17 companies met investor criteria; highest valuations in USA, China, India, UK, Germany

## Example Insights

- Europe and Middle East show high unicorn activity and investor interest  
- Row deletion causes less data loss than column deletion  
- Imputed values are reasonable but may need manual checks

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
