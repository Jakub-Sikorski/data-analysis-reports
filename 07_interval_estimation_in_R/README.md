# Interval Estimation & Confidence Intervals in R

## Project Description
This project focuses on interval estimation and the practical evaluation of confidence intervals under various conditions. Using R and R Markdown, the report explores population parameter estimation for means, variances, and proportions through extensive Monte Carlo simulations, culminating in a real-world application using economic data.

## Technologies Used
* **R:** Core programming language for statistical simulations and data processing.
* **R Markdown:** Used to generate a reproducible and professional PDF report.
* **Base R Graphics:** Employed to create custom coverage probability plots, histograms, and Q-Q plots for distributional checks.

## Methodology
The analytical workflow is divided into three main sections:
1. **Confidence Intervals for Means and Variances:** Simulating data from normal and Student's t-distributions across 1,000 replications to evaluate coverage probabilities and robustness against non-normality.
2. **Proportion Estimation:** Comparing the coverage performance of the traditional Wald confidence interval versus the Agresti-Coull interval for binomial proportions $B(1, \theta)$ across varying sample sizes and extreme probabilities.
3. **Real-World Application & CLT Verification:** Applying interval estimation to the US income dataset to verify coverage rates for skewed population data and illustrating the Central Limit Theorem via distribution convergence.

## Key Findings
* **Robustness of the Mean vs. Variance:** The classical confidence interval for the mean is robust against non-normality. Conversely, the standard interval for variance completely breaks down when underlying data deviates from normality, showing severely degraded coverage.
* **Superiority of Agresti-Coull:** The traditional Wald interval for proportions struggles near boundary values in small samples. The Agresti-Coull interval maintains stable coverage close to the nominal 95% level across all parameter spaces.
* **Central Limit Theorem in Action:** Applying repeated sampling to a heavily right-skewed income distribution demonstrates that as sample size increases from $n = 50$ to $n = 200$, the distribution of sample means rapidly converges to normality, as verified by Q-Q plots.

## File Structure
* `Raport4.Rmd` - The R Markdown source file containing all simulation code and descriptive text.
* `Raport4.pdf` - The final compiled PDF report.
* `income.dat` - The real-world dataset used for the economic parameter estimation task.
