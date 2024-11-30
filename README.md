# Bacteria-Dynamics
Modeling *Pseudomonas aeruginosa* and *Staphylococcus aureus*

---

## Bacterial Growth Models

### Overview
This repository contains predictive models for the theoretical growth and decay of two bacterial species:
- *Pseudomonas aeruginosa*
- *Staphylococcus aureus*

These models simulate bacterial growth under idealized conditions using the logistic growth equation and bacterial reduction based on radiation dose using a decay model.

---

### Features
- Predicts bacterial population growth over time.
- Models bacterial reduction due to radiation dose.
- Visualizes logistic growth curves and decay trends.

---

### Assumptions

#### Parameters for *Pseudomonas aeruginosa*
- Initial concentration (\(N_0\)): \(10^3\) CFU/mL
- Maximum concentration (\(N_{\text{max}}\)): \(1.67e13\) CFU/mL
- Growth rate (\(r\)): 0.45 hour\(^{-1}\)

#### Parameters for *Staphylococcus aureus*
- Initial concentration (\(N_0\)): \(10^3\) CFU/mL
- Maximum concentration (\(N_{\text{max}}\)): \(5.96e12\) CFU/mL
- Growth rate (\(r\)): 0.40 hour\(^{-1}\)

#### Radiation Decay Model Parameters
- **Initial CFU Count (\( \text{max\_cf} \))**: Maximum bacterial count before radiation.
- **Half-Max Dose (\( \text{half\_max\_dose} \))**: The dose at which bacterial CFUs reduce to half.
- **Steepness (\( \text{steepness} \))**: Controls the steepness of the decay curve.

---

### Decay Model Explanation

The bacterial decay due to radiation is modeled using a logistic decay function. The function calculates the CFU count as a function of the applied radiation dose. The formula used is:

\[
CFU = \text{max\_cf} \cdot \left(1 - \frac{1}{1 + e^{-\text{steepness} \cdot (\text{dose} - \text{half\_max\_dose})}}\right)
\]

#### Parameters:
- **max\_cf**: Initial bacterial CFU count (e.g., \(300\)).
- **dose**: Radiation dose(s) applied to the bacteria.
- **half\_max\_dose**: Dose where CFU count is reduced to half.
- **steepness**: Steepness of the decay curve (higher value = steeper decay).

#### Implementation:
The code calculates CFUs across a range of radiation doses and plots the decay trend.

---

### Prerequisites
- Python 3.x
- Required libraries:
  - `numpy`
  - `matplotlib`

Install dependencies with:
```bash```
pip install numpy matplotlib

## License

This project is licensed under the MIT License.

## Contact

For questions please reach out to knowle.marcus@utexas.edu
