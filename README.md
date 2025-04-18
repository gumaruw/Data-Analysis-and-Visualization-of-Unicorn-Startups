# 🦄 Unicorn Companies Missing Data Handling

> This project was completed as part of my scholarship in the Data Science program at the Artificial Intelligence and Technology Academy. It was undertaken within the scope of the "Go Beyond the Numbers: Translate Data into Insights" chapter of the Google Advanced Data Analytics course.

## 📊 Overview

This project involves data analysis with a focus on handling missing data within a dataset related to unicorn companies, including their funding, valuation, and geographic distribution. The primary objectives were to:

- Detect and handle missing data effectively.
- Visualize key insights, such as the highest valued countries and the sectors that attract investors.
- Understand the impact of missing data handling techniques on the analysis results.

## 📁 Dataset

- **Name:** `Unicorn_Companies.csv`
- **Source:** Kaggle
- **Rows:** 1,074 unicorn companies
- **Columns:** 10 (including company name, valuation, funding, industry, investors, etc.)

### Key Columns:

- `Company`: Name of the unicorn company  
- `Valuation`: Company valuation (in billions)  
- `Date Joined`: Date the company became a unicorn  
- `Industry`: Business industry  
- `Funding`: Total funding raised  
- `Year Founded`: Year the company was founded  
- `Select Investors`: Top investors  
- `Country/Region`, `Continent`, `City`: Geolocation details  

## 🛠 Technologies Used

- **Python**
- **Pandas**
- **Matplotlib**
- **Jupyter Notebook**

## 🧪 Key Steps Taken
1. **Missing Data Detection**:  
   Missing data was identified using the `isna()` function, and rows containing at least one missing value were filtered using `any(axis=1)`.

2. **Handling Missing Data**:  
   - Dropped rows with missing values when the missing data was minimal.
   - Imputed missing values in certain columns (like Funding and Select Investors) with default values or categories.
   - Explored alternative imputation methods such as using the mean/mode or prediction models.

3. **Data Visualization**:  
   - Visualized the valuation of unicorns by country using circle charts where the circle size represents the total unicorn valuation for each country.
   - Analyzed the highest performing regions, with a particular focus on Europe and the Middle East.

4. **Analysis Results**:  
   - Identified 17 companies that met investor criteria.
   - Observed that the highest total valuations are found in countries like the USA, China, India, the UK, and Germany.

## 📈 Example Insights

- The dataset revealed that certain regions, especially Europe and the Middle East, show high activity in terms of unicorns and investor interest.
- Handling missing data, specifically through row deletion, resulted in less data loss compared to column deletion.
- The imputed values were largely reasonable, but manual verification may still be necessary for more accurate results.

## ✅ Outcome

By the end of this project, we were able to:

- Conduct exploratory data analysis (EDA) and handle missing values through removal and imputation.
- Filter unicorn companies based on industry, city, and valuation.
- Transform data, create new columns, and prepare it for analysis.
- Generate visualizations to highlight trends in the global unicorn market.
- Provide actionable insights to the investor with interactive maps and country-specific valuations.

## 📌 How to Run

1. Clone the repository  
2. Open the Jupyter Notebook file  
3. Ensure that `Unicorn_Companies.csv` is in the same directory  
4. Run the notebook step-by-step

```bash
git clone https://github.com/gumaruw/Unicorn-Companies-Missing-Data-Handling.git
cd Unicorn-Companies-Missing-Data-Handling
jupyter notebook
```

## 📌 Additional Notes
This project showcases the impact of missing data handling and provides actionable insights that could help investors identify high-potential countries and sectors. The project also offers valuable experience in data preprocessing, cleaning, and visualization techniques.

## ⚖️ License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
