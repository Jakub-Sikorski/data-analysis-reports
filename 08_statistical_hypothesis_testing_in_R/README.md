# Statistical Hypothesis Testing & Medical Data Analysis in R

## Project Description
This project focuses on the theory and practical application of statistical hypothesis testing. It is divided into two main parts: a theoretical simulation study to explore the distribution of p-values, Type I errors, and statistical power under varying conditions, and a practical application on a real-world medical dataset. The practical section involves visually and statistically analyzing cholesterol levels between heart attack patients and a healthy control group, including a manual implementation of Welch's t-test from scratch to verify mathematical comprehension.

## Technologies Used
* **R:** Programming language used for simulations, statistical testing, and data manipulation.
* **R Markdown:** Used to compile the analysis, equations, and visualizations into a comprehensive PDF report.
* **Base R Graphics & `car` Package:** Employed for generating histograms, Q-Q plots, distribution curves, and comparative boxplots.

## Methodology
The analysis is structured around the following key areas:
1. **P-value Distribution & Type I Error:** Simulating data from a standard normal distribution to verify that p-values follow a uniform distribution and to estimate the empirical Type I error rate.
2. **Statistical Power Simulations:** Simulating data under $H_1$ to visualize the heavily skewed p-value distribution. Further analysis includes generating theoretical curves to demonstrate how statistical power varies with changes in the effect size, sample size ($n$), and population variance ($\sigma^2$).
3. **Medical Data Analysis:** Utilizing boxplots to track cholesterol trends in patients post-myocardial infarction and comparing them against a healthy control group.
4. **Algorithmic Implementation:** Manually coding the mathematical formula for Welch's t-test (handling unequal variances and adjusting degrees of freedom) and comparing the outputs against R's built-in `t.test()` function to ensure absolute computational accuracy.

## Key Findings
* **Power Dynamics:** The theoretical curves confirmed that the power of a statistical test increases rapidly as the true mean deviates further from the null hypothesis, and as the sample size grows. Conversely, increased data variance introduces "noise," significantly reducing the test's power.
* **Clinical Insights:** The graphical analysis revealed a clear downward trend in cholesterol levels for heart attack patients over the 14-day observation period. However, their initial levels were substantially higher and more dispersed than those of the control group.
* **Statistical Significance & Verification:** Welch's t-test confirmed a highly statistically significant difference in cholesterol levels between patients on Day 2 post-infarction and the control group. The manual implementation of the test yielded results identical to the built-in R function down to the last decimal, validating the underlying mathematical logic.

## File Structure
* `Raport5.Rmd` - The R Markdown source file containing the hypothesis testing simulations and custom function code.
* `Raport5.pdf` - The compiled report detailing the findings and visualizations.
* `chol.txt` - The medical dataset containing cholesterol measurements over time for patient and control groups.
