# Forensic Application of Newton's Law of Cooling

## Project Description
This project demonstrates the practical application of first-order differential equations in the field of forensic science. By utilizing Newton's Law of Cooling, the project models the heat transfer of a human body to accurately estimate the time of death based on temperature measurements taken at the crime scene. 

## Technologies Used
* **R:** Core programming language for mathematical modeling and calculations.
* **R Markdown:** Used to create a structured and reproducible PDF report, incorporating mathematical formulas using LaTeX.
* **Base R Graphics:** Employed to generate the cooling curve visualization, highlighting key events.
* **LaTeX:** Typesetting mathematical equations for the general and particular solutions of the differential equation.

## Methodology
The workflow is divided into the following steps:
1. **Mathematical Modeling:** Deriving the general and particular solutions for the temperature function $T(t)$ by solving the first-order differential equation for Newton's Law of Cooling using the separation of variables method.
2. **Data Input & Parameter Estimation:** Using theoretical crime scene data to calculate the specific cooling constant.
3. **Time of Death Calculation:** Reversing the temperature function to estimate the exact time elapsed since death.
4. **Data Visualization:** Plotting the exponential cooling curve of the body, visually mapping out the moment of death against the timeline of the investigation.

## Key Findings
* **Mathematical Precision:** The model successfully calculated the cooling constant and determined that the time of death occurred approximately 2 hours and 3 minutes before the body was found.
* **Model Limitations:** While the model provides a strong foundation for forensic analysis, real-world applications require accounting for dynamic variables, such as fluctuating ambient temperatures and changing cooling rates, which are simplified in this specific first-order differential model.

## File Structure
* `projekt.Rmd` - The R Markdown source file containing the LaTeX equations, R code, and analysis text.
* `projekt.pdf` - The final compiled PDF report.
