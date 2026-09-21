# Numerical Methods: Bisection, Monte Carlo & Trapezoidal Rule in R

## Project Description
This project demonstrates the practical application of fundamental numerical methods implemented in R. It explores algorithms for root-finding (Bisection Method) and numerical integration. The report evaluates the accuracy, efficiency, and impact of key parameters (such as the number of subintervals or sample sizes) on computational results.

## Technologies Used
* **R:** Core programming language for implementing numerical algorithms.
* **R Markdown:** Used to generate a clean and reproducible PDF report incorporating mathematical notation via LaTeX.
* **Base R Graphics:** Employed to visualize functions, root-finding intervals, random sampling areas (Monte Carlo), and geometric trapezoids under the curve.

## Methodology
The analysis is structured around three core numerical techniques:
1. **Bisection Method:** Iteratively narrowing down an interval where a function changes sign to find a root based on a specified tolerance.
2. **Monte Carlo Integration:** Estimating definite integrals by randomly sampling points within a bounding box and calculating the proportion of points falling under the curve.
3. **Trapezoidal Rule:** Approximating the area under a curve by dividing the integration interval into smaller subintervals and summing the areas of the resulting trapezoids.

## Key Findings
* **Bisection Stability:** The bisection method proved to be extremely stable and guaranteed convergence given a sign change, though it exhibits slower convergence compared to derivative-based methods.
* **Monte Carlo Universality:** Monte Carlo integration proved to be highly versatile, especially for complex domains, though its accuracy scales relatively slowly.
* **Trapezoidal Efficiency:** The trapezoidal rule achieved high accuracy very quickly for smooth functions, reaching the target error threshold with a relatively small number of subdivisions.

## File Structure
* `s_354584.Rmd` - The R Markdown source file containing the custom algorithms, code, and analysis text.
* `s_354584.pdf` - The final compiled PDF report.
