# Bacteria-Dynamics
Modeling P. Aeruginosa and S. Aereus 

# Bacterial Growth Models

## Overview
This repository contains predictive models for the theoretical growth of two bacterial species:
- *Pseudomonas aeruginosa*
- *Staphylococcus aureus*

These models simulate bacterial growth under idealized conditions using the logistic growth equation.

## Features
- Predicts bacterial population growth over time.
- Visualizes the logistic growth curves.
- Models use assumed growth parameters derived from typical bacterial growth dynamics.

## Assumptions
### Parameters for *Pseudomonas aeruginosa*
- Initial concentration (\(N_0\)): \(10^6\) CFU/mL
- Maximum concentration (\(N_{\text{max}}\)): \(10^9\) CFU/mL
- Growth rate (\(r\)): 0.5 day\(^{-1}\)

### Parameters for *Staphylococcus aureus*
- Initial concentration (\(N_0\)): \(10^5\) CFU/mL
- Maximum concentration (\(N_{\text{max}}\)): \(10^8\) CFU/mL
- Growth rate (\(r\)): 0.4 day\(^{-1}\)

## Prerequisites
- Python 3.x
- Required libraries:
  - `numpy`
  - `matplotlib`

Install dependencies with:
```bash
pip install numpy matplotlib

## Usage
Run the respective Python script for each bacterial species:

python pseudomonas_model.py
python staphylococcus_model.py

The script will generate and display the growth curve.

## Output

- **Growth Curve**: A plot showing bacterial population growth over time.
- **Predicted Parameters**:
  - Carrying capacity (\(N_{\text{max}}\))
  - Growth rate (\(r\))
  - Time to reach carrying capacity.

## Example Results

### *Pseudomonas aeruginosa*
- Growth starts at \(10^6\) CFU/mL.
- Reaches a maximum population of \(10^9\) CFU/mL in ~12–15 days.

### *Staphylococcus aureus*
- Growth starts at \(10^5\) CFU/mL.
- Reaches a maximum population of \(10^8\) CFU/mL in ~13–15 days.

## License

This project is licensed under the MIT License.

## Contact

For questions please reach out to knowle.marcus@utexas.edu


