# Unseen Species Index

This directory contains notebooks implementing the unseen species model, which is used to estimate cultural diversity and production potential based on historical data.

## Directory Structure

- **data/** - Directory for storing input and output datasets
- **unseen_species_model/** - Contains the final model outputs and parameter estimates

## Notebooks

1. **1-prepare_dataset.ipynb**  
   Prepares and processes the raw data into a format suitable for the unseen species modeling. This includes data cleaning, normalization, and structuring the time series data.

2. **2-run_generalized_chao_model.ipynb**  
   Implements and runs the generalized Chao model for estimating unseen species. This notebook applies statistical methods to estimate the number of "unseen" cultural productions based on observed patterns.

3. **3-extract_model_table.ipynb**  
   This notebook generates the key metrics and findings from the model.

4. **4-estimator_robustness_analysis.ipynb**  
   Compare different diversity estimators

## Key Output

The primary output of this analysis pipeline is in:

```
unseen_species_model/unseen_species_model_bayesian.csv
```

This file contains the Bayesian model estimates for cultural diversity across different regions and time periods.

## Usage

These notebooks should be run sequentially as each depends on the outputs of the previous steps.

Requirements:

- For the Bayesian computations in these notebooks (especially in notebook 2), a GPU is recommended for reasonable performance
- The bambi package is used for Bayesian modeling

## Methodology

The unseen species model adapts ecological diversity estimation techniques to cultural production data. It estimates the "unseen" cultural productions that likely existed but weren't recorded in historical catalogs, providing a more complete picture of cultural diversity across regions and time periods.
