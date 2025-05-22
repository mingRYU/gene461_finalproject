# gene461_finalproject
## Project Summary

This project explores how to model and classify cell population growth dynamics using both simulated and real single-cell RNA sequencing (scRNA-seq) data. We developed a pipeline that simulates cell populations under different growth regimes, extracts graph-based and topological features from simulated differentiation trajectories, and trains classifiers (e.g., Graph Convolutional Networks and Random Forests) to distinguish among growth types.

We then applied this framework to real hematopoietic stem cell (HSC) data from the Human Cell Atlas to infer the underlying population dynamics of immune cell development. The goal is to assess whether computational classifiers trained on synthetic data can generalize to real biological systems and provide insights into self-renewal and differentiation behavior in hematopoiesis.

A document containing derivations (based on branching process) on the expected distribution for each growth regime is also included: branching_results_outline.pdf

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
