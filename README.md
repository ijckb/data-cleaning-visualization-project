# Data Cleaning & Visualization Project

A data analysis project that cleans and explores the Titanic dataset using Python, uncovering patterns in passenger survival through visualization.

## 📌 Project Overview
This project works through a raw dataset to handle missing values, duplicates, and outliers, then uses visualizations to extract and communicate insights.

## 🛠 Tools & Libraries
- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook (via VS Code)

## 📂 Files
- `analysis.ipynb` — main notebook with all cleaning, analysis, and visualization code
- `README.md` — project documentation

## 🧹 Data Cleaning Steps
- Dropped the `deck` column (688 of 891 values missing — too sparse to be useful)
- Filled missing `age` values (177 missing) using the median
- Filled missing `embarked` and `embark_town` values (2 each) using the mode
- Checked for duplicate rows — none found
- Reviewed `fare` for outliers using a boxplot; retained legitimate high-value first-class fares

## 📊 Visualizations
- Survival count (overall)
- Survival by gender
- Survival by passenger class
- Age distribution
- Correlation heatmap of numeric features
- Age vs. Fare scatter plot, colored by survival

## 🔎 Key Insights
- Women had a significantly higher survival rate than men
- 1st class passengers survived at much higher rates than 2nd or 3rd class
- Most passengers were between ages 20–40
- Higher fares (linked to passenger class) correlated with better survival odds
- Age alone was a weaker predictor of survival compared to class and fare

## ▶️ How to Run
1. Clone this repository:
```bash
   git clone https://github.com/ijckb/data-cleaning-visualization-project.git
```
2. Install dependencies:
```bash
   pip install pandas numpy matplotlib seaborn jupyter
```
3. Open `analysis.ipynb` in Jupyter Notebook or VS Code and run all cells

## 📈 Outcome
This project demonstrates core data preprocessing techniques (handling missing data, duplicates, and outliers) alongside exploratory data analysis and storytelling through visualization.