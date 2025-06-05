# Cultura

[![PyPI - Python](https://img.shields.io/badge/python-v3.9-blue.svg)](https://pypi.org/project/bunkatopics/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.10-blue.svg)](https://pypi.org/project/bunkatopics/)
[![PyPI - Python](https://img.shields.io/badge/python-v3.11-blue.svg)](https://pypi.org/project/bunkatopics/)

<img src="images/Cultura 1.0 - cultura_logo.png" width="50%">

This repository contains the code for the paper "Cultural Production Reveals Transitions to Sustained Growth Development in both European and Non-European Societies." The repository provides tools and scripts for extracting, analyzing, and visualizing cultural data from the 'Cultura' database.

## Repository Structure

The project is organized into 5 main components, each handling a different aspect of the analysis:

1. **cultura_database_creation** - Scripts for creating and initializing the primary database used in the study
2. **cultura_database_extract** - Tools for extracting and processing data from the primary database
3. **unseen_species_index** - Use of tools from ecololgy to estimate the cultural diversity
4. **CPM_index** - Cultural Production Metrics index calculation and analysis
5. **CPM_HDI_GDPpc_relationship** - Analysis examining relationships between Cultural Production Metrics, Human Development Index, and GDP per capita

## Getting Started

Most scripts are Notebooks.

### Prerequisites

- Python 3.9+ (compatible with 3.9, 3.10, 3.11)
- Jupyter Notebook

### Hardware Requirements

For Bayesian computations related to the unseen species models (with the bambi package) a GPU is advised to speed up the process. The rest of the analysis can be conducted on any standard computer with sufficient RAM to support the in-memory operations.

### Python Dependencies

Cultura mainly depends on few packages:

- sqlite3
- statsmodels
- bambi
- pandas
- matplotlib
- arviz
- numpy
- seaborn
- adjustText
- tqdm
- dotenv
- scipy
- copia
- sparqlwrapper
- pydantic

### Installation

```bash
# Clone the repository
git clone https://github.com/charlesdedampierre/cultura.git
cd cultura

# Create and activate a virtual environment (recommended)
python3 -m venv cultura_env
source cultura_env/bin/activate  # On Windows, use: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Usage

The analysis is performed sequentially through Jupyter notebooks in each directory. For detailed instructions, please refer to the README files in each repository:

1. [cultura_database_creation](1-cultura_database_creation/README.md)
2. [cultura_database_extract](2-cultura_database_extract/README.md)
3. [unseen_species_index](3-unseen_species_index/README.md)
4. [CPM_index](4-CPM_index/README.md)
5. [CPM_HDI_GDPpc_relationship](5-CPM_HDI_GDPpc_relationship/README.md)

## Data

The Cultura database can be downloaded from the Open Science Framework (OSF): <https://osf.io/d78tw>

After downloading the database, set up the environment variable to access it:

```bash
export DB_PATH="/path/to/your/cultura_03_2025.db"
```

## License

This project is licensed under the MIT Licence

## Contact

[Charles de Dampierre] - [charlesdedampierre@gmail.com]
