# gene461_finalproject

This repository contains code and analysis for simulating cell population dynamics, extracting features, and training classifiers to predict growth regimes, as part of the final project for GENE 461.

## Notebooks

### 1. `simulate_and_train.ipynb`
- Generate parameters for different dynamical systems
- Run simulations of cell population dynamics
- Extract numerical features from each simulated cell population
- Train a classifier (Graph CNN or Random Forest) to predict the growth regime label

### 2. `simulate_HSC.ipynb`
- Simulate three cell populations with different growth regimes
- Visualize all populations in a common PCA plot
- Use the trained classifier to predict the growth regime for each simulated population

### 3. `scRNA_li_HICA.ipynb`
- Analyze Hematopoietic Stem Cells (HSCs) using scRNA-seq data from the Human Cell Atlas  
  [Data source: HCA project link](https://explore.data.humancellatlas.org/projects/cc95ff89-2e68-4a08-a234-480eca21ce79)
- Extract HSCs and derived immune cells from the bone marrow of individual donors
- Predict population growth dynamics using the trained classifier
