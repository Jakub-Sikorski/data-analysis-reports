# Statistical Theorems Simulation: LLN & CLT

## Project Description
This project focuses on simulating and visually verifying two fundamental laws of mathematical statistics: the Law of Large Numbers and the Central Limit Theorem. By combining theoretical probability experiments with real-world dataset applications, the report provides a hands-on demonstration of statistical convergence and sampling distributions. 

## Technologies Used
* **R:** Core programming language for statistical computing and simulations.
* **R Markdown:** Used to create a reproducible and structured PDF report.
* **Base R Graphics:** Employed to generate histograms, line charts, and distribution curves for visual verification of the theorems.

## Methodology
The analytical workflow is divided into three main parts:
1. **Law of Large Numbers:** Simulating classic random experiments to observe how the sample mean converges to the theoretical expected value as the sample size increases.
2. **Central Limit Theorem:** Drawing samples from highly skewed and discrete (Poisson) distributions to visualize the standardized sample mean converging to a Standard Normal Distribution $N(0,1)$.
3. **Real-World Application:** Applying the theorems to a US Income dataset (`income.dat`) to demonstrate how sample means approximate the true population mean, and verifying the theoretical standard error formula.

## Key Findings
* **LLN in Practice:** Initial small samples exhibit high variance, but as the number of trials increases (e.g., approaching $n=100$), the sample mean strictly stabilizes around the theoretical expected value.
* **CLT Verification:** Regardless of the underlying distribution's shape (whether heavily skewed or discrete), increasing the sample size smooths the data into a classic symmetric "bell curve" that aligns with the standard normal density line.
* **Sampling Precision:** In the income dataset, scaling the sample size by a factor of 100 resulted in exactly a tenfold decrease in the theoretical standard deviation of the sample mean, perfectly validating the mathematical formula $\frac{\sigma}{\sqrt{n}}$.

## File Structure
* `Raport2.Rmd` - The R Markdown source file containing the simulation code and analysis text.
* `Raport2.pdf` - The final compiled report document.
* `income.dat` - The real-world demographic dataset used for the final practical application.
