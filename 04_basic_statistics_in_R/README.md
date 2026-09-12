# Exploratory Data Analysis & Basic Statistics in R

## Project Description
This project demonstrates fundamental statistical analysis and data visualization using R and R Markdown. It explores two distinct datasets: US student performance metrics (grades, IQ, psychological tests) and US citizens' income data from the year 2000. The primary focus is on understanding data distributions, identifying skewness and outliers, and performing comparative group analyses to extract meaningful insights.

## Technologies Used
* **R:** Core programming language for statistical computing.
* **R Markdown:** Used for creating a dynamic, reproducible, and aesthetically pleasing PDF report.
* **Base R Graphics:** Generating histograms and boxplots for data visualization.

## Methodology
The analytical workflow is structured around the following key areas:
1. **Descriptive Statistics:** Calculating and interpreting measures of central tendency (mean, median) and dispersion (variance, standard deviation, coefficient of variation) to understand the shape of the data.
2. **Visual Analysis & Outlier Handling:** Utilizing histograms to evaluate distributions—including an experiment on how the number of bins (`breaks`) impacts data readability—and boxplots to identify and manage extreme outliers.
3. **Comparative Analysis:** Evaluating statistical differences between groups, specifically analyzing performance and psychological traits by gender, and examining the relationship between education levels and income.
4. **Robust Statistics:** Applying a 10% trimmed mean to heavily right-skewed financial data to mitigate the impact of extreme outliers and establish a more realistic "average" income metric.

## Key Findings
* **Student Data:** Grades and psychological test scores exhibit a left-skewed distribution. While median grades are almost identical across genders, boys showed a wider variance and slightly higher average IQ scores within this specific sample.
* **Income Data:** The US income distribution in 2000 was severely right-skewed. Visualizations without outliers clearly demonstrate a strong positive correlation between education level and income, with a particularly notable jump for university graduates. Furthermore, the analysis revealed a significant wage gap, with men earning substantially more than women across the board.
* **Methodological Insight:** For highly skewed financial data, the classical arithmetic mean is heavily distorted by top earners. The 10% trimmed mean proved to be a much more accurate reflection of the typical citizen's earnings.

## File Structure
* `Raport1.Rmd` - The R Markdown source file containing the code and analysis text.
* `Raport1.pdf` - The final compiled report document.
* `grades.txt` - Dataset containing student metrics.
* `income.dat` - Dataset containing US income and demographic data.
