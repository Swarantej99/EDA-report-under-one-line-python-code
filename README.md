#  Generate a Full EDA Report in One Line of Python( Within a minute)

**AutoEDA** is a lightweight Python project/discovery that showcases how you can generate an entire Exploratory Data Analysis (EDA) report — complete with summary statistics, visualizations, and diagnostics — using just a **single line of code**.  

It’s a practical demonstration of making data profiling fast, repeatable, and integrable into data workflows and pipelines.

---

## Project Motivation

- Performing EDA manually across dozens or hundreds of features is time-consuming and error-prone  
- Visualizing distributions, correlations, missing values, and data quality checks often requires writing many lines of code  
- AutoEDA condenses that into one command that handles the heavy lifting, gives interactive insight, and accelerates the data exploration process

---

## Features & Highlights

- One-liner execution: `AutoEDA(df)` or `ProfileReport(df)` generates a full HTML report  
- Automatically examines distributions, correlations, missing values, duplicates, skewness, and variable types  
- Supports both numerical and categorical features  
- Interactive HTML output, easy to share or embed  
- Can be integrated into ETL pipelines or data validation workflows  

---

## How It Works (Internals)

- Wraps **`ydata-profiling` (formerly pandas-profiling)** under a convenience interface  
- Passes your `pandas.DataFrame` to internal functions that compute:
  1. Summary statistics (mean, std, quartiles, etc.)  
  2. Feature correlations and pairwise relationships  
  3. Missing values, duplicates, and data quality indicators  
  4. Histograms, boxplots, and distribution visuals  
- Renders the final report as an interactive HTML file or inline notebook display  

---

## Installation & Usage

```bash
pip install pandas ydata-profiling
