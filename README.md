# EDA & Hypothesis Testing on a Restaurant Tips Dataset

Exploratory data analysis and statistical hypothesis testing in Python.

**Dataset:** `tips.csv` - 244 restaurant bills (total_bill, tip, sex, smoker, day, time, size). Source: [seaborn-data](https://github.com/mwaskom/seaborn-data).

## What is done
- Data cleaning: missing values, duplicate removal, type conversion, IQR outlier check
- Feature engineering: tip percentage
- EDA: distributions, box plots, scatter plot, correlation heatmap, group-wise means
- Hypothesis tests: Pearson correlation, Welch t-test (smoker, sex), one-way ANOVA + Kruskal-Wallis (day), Shapiro-Wilk normality check, confidence interval for a difference in means

## Key findings
- Tip amount and total bill are strongly correlated (r = 0.675, p < 0.001)
- No significant difference in tip percentage by smoker status, sex or day (all p > 0.05)

## Run it
```
pip install -r requirements.txt
jupyter notebook EDA_Hypothesis_Testing_Tips.ipynb
```
