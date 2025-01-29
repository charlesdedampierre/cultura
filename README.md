# Cultura

[![PyPI - Python](https://img.shields.io/badge/python-v3.9-blue.svg)](https://pypi.org/project/bunkatopics/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.10-blue.svg)](https://pypi.org/project/bunkatopics/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.11-blue.svg)](https://pypi.org/project/bunkatopics/)

<img src="images/Cultura 1.0 - cultura_logo.png" width="20%">

This repository contains the code for the paper "Cultural Production Reveals Transitions to Sustained Growth Development in both European and Non-European Societies." The repository provides tools and scripts for extracting, analyzing, and visualizing cultural data from the 'Cultura' database.

Most scripts are Notebooks.

The main data from the unseen-species model are in the following file:

'unseen_species_model/unseen_species_model_bayesian.csv'

## Cultura database

The database used in that project can be extracted here: <https://osf.io/2euxr/>

Add the environement of the cultura database to access it

```bash
export DB_PATH="/path/to/your/cultura.db"
```

### Hardware Requirements

For Bayesian computations related to the unseen species models (with the bambi package)(in 6c - run_best_model_north_south.ipynb), a GPU is needed. The rest of the analysis can be conducted on any standard computer with sufficient RAM to support the in-memory operations.

### Python Dependencies

Cultura mainly depends on few packages

- sqlite3
- statsmodels
- bambi
- pandas
- matplotlib
- arviz
- numpy
