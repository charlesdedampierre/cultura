# Cultura Database Extract

This directory contains notebooks for extracting and analyzing data from the Cultura database. These notebooks process raw database content into structured datasets for further analysis.

## Directory Structure

- **data/** - Directory for storing additional datasets
- **db_extract/** - Scripts for database extraction utilities

## Notebooks

**1-make_individuals_and_regions_score copy.ipynb**  
Creates individual and regional scoring metrics based on the cultural production data in the database.

**2-extract_CPs_works.ipynb**  
Extracts Cultural Production (CP) works from the database for analysis.

**3-stats_by_catalog.ipynb**  
Generates statistical analysis of cultural productions grouped by catalog sources.

**3b-stats_works.ipynb**  
Provides additional statistical analysis focused on cultural works.

**4-wikipedia_creation_date.ipynb**  
Analyzes creation dates of cultural works as reported in Wikipedia sources.

**5-online_catalogs_trends.ipynb**  
Examines trends in online catalogs of cultural productions over time.

**6-extract_works_databases.ipynb**  
Extracts detailed work information from various database sources.

**7-unique_vs_multi_contributors.ipynb**  
Analyzes the patterns of unique versus multiple contributors to cultural works.

**9-extract_social_origins_pilot.ipynb**  
Pilot for the social origins of Cultural Producers

**9-extract_social_origins.ipynb**  
Extarction of the social origins using the API of GPT4

**10-graph_social_origins.ipynb**  
Graph for the social origins

**11-evaluation_social_origins.ipynb**  
Computing metrics to evaluate the sample annotated to check the effectiveness of GPT-4 annotation

## Usage

These notebooks should be run in numerical order.

To run these notebooks, make sure you have:

1. Downloaded the Cultura database from OSF
2. Set up the environment variable:

    ```bash
    export DB_PATH="/path/to/your/cultura.db"
    ```

The Script number requires an OpenAI key
