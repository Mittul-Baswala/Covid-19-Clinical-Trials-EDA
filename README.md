# 🦠 COVID-19 Clinical Trials Exploratory Data Analysis (EDA)

## 📌 Project Overview
This project is an **Exploratory Data Analysis (EDA)** of a dataset containing information on clinical trials registered for COVID-19 treatments, diagnostics, and prevention measures.  

The primary goal is to:
- Understand the structure of the dataset  
- Clean and preprocess the data  
- Extract key insights regarding the distribution of trials, their status, geographical spread, and timeline of initiation  

---

## 📊 Key Analyses & Findings
The analysis was performed in the accompanying Jupyter Notebook: **`covid-19 clinical trials.ipynb`**

- **Data Loading & Exploration**  
  - Loaded dataset with **5,783 rows** and **27 columns**  
  - Inspected structure, column information, and sample records  

- **Missing Data Handling**  
  - Calculated missing value percentages per column  
  - Visualized missing data using a heatmap  
  - Dropped columns with very high missing rates:  
    - `Results First Posted` (99.4%)  
    - `Study Documents` (96.9%)  
  - Imputed missing categorical values (`Acronym`, `Phases`, `Interventions`, `Locations`, etc.) with `"Unknown"`  
  - Handled skewed `Enrollment` column (skewness = 34.07) by imputing with the **median (170.0)**  

- **Feature Engineering**  
  - Created a new `Country` column by extracting country names from `Locations` for geographical analysis  

- **Data Visualization (Key Insights)**  
  - **Top 10 Countries by Trials**: Countries with the highest number of registered clinical trials  
  - **Distribution of Trial Status**: Recruiting, Active (not recruiting), Completed, etc.  
  - **Gender Distribution**: Trials targeting Male, Female, or All participants (pie chart)  
  - **Trial Initiation Timeline**: Cumulative growth of clinical trials over time  
  - **Heatmap of Trial Status by Country**: Breakdown of trial statuses within top 10 contributing countries  
  - **Trials Started by Month**: Monthly counts showing peak periods of research activity  

---

## 🛠 Technologies & Libraries
- **Python**  
- **Pandas** → Data manipulation & cleaning  
- **NumPy** → Numerical operations  
- **Matplotlib & Seaborn** → Data visualization  

---ps://github.com/yourusername/covid19-clinical-trials-eda.git
