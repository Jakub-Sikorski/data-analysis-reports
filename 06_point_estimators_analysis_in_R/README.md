# Point Estimators Analysis in R

## Project Description
This project investigates the mathematical properties and practical behavior of various statistical point estimators under different conditions. The report is divided into three main sections: evaluating estimators of the expected value, testing estimator robustness against extreme outliers, and comparing estimators of variance. By simulating data from normal distributions with varying parameters and sample sizes, this project provides a visual and quantitative assessment of estimator bias, variance, and Mean Squared Error.

## Technologies Used
* **R:** Core programming language for statistical simulations and calculations.
* **R Markdown:** Used to create a structured, reproducible PDF report.
* **Base R Graphics:** Employed to generate boxplots and line charts for visual comparison of estimators.

## Methodology
The analysis is structured around the following key experiments:
1. **Expected Value Estimators:** Comparing four estimators—Arithmetic Mean, Median, Midhinge, and Trimmed Mean—across different population parameters and sample sizes.
2. **Robustness to Outliers:** Introducing an extreme value to a sample and calculating the bias, variance, and MSE of both the arithmetic mean and the median to evaluate their resilience to data anomalies.
3. **Variance Estimators:** Analyzing three different methods of estimating sample dispersion: classic Sample Variance, variance calculated using the median, and the median of squared deviations.

## Key Findings
* **Optimal Expected Value Estimation:** In a perfectly normal distribution without anomalies, the classical arithmetic mean is the most efficient estimator, consistently achieving the lowest Mean Squared Error compared to the median, trimmed mean, or midhinge.
* **Outlier Robustness:** The arithmetic mean is highly sensitive to outliers; introducing just one extreme value causes its MSE to skyrocket linearly. Conversely, the median is a robust estimator that remains perfectly stable and unbiased regardless of extreme outliers.
* **Variance Estimation:** The classic sample variance and the variance based on the median are unbiased and highly accurate estimators of population variance. On the other hand, the median of squared deviations proved to be severely biased, heavily underestimating the true variance even as the sample size increased.

## File Structure
* `Raport3.Rmd` - The R Markdown source file containing the simulation logic, code, and analysis text.
* `Raport3.pdf` - The final compiled report document.
