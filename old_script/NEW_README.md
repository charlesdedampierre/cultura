
# Database Stats

Scriptsq that tackles the Cultura DB as input and outputs some analysis on individuals and works

Input:
    cultura_database
Output:
    data/
    figures/

- [CPs Extraction](<../1 - make_individuals_and_regions_score.ipynb>)
-->  'db_extract/df_individuals_score.csv'

Comment: some manual change to describe

- [CPs Works Extraction](<../2 - extract_CPs_works.ipynb>)

Input:

-->  'db_extract/df_individuals_score.csv'
-->  'cultura_database

Output:

--> df_indi_works.csv
--> df_indi_works_occupations.csv

Comment: we lose individuals with the top occupations

- [Catalogs Stats](<../3 - stats_by_catalog.ipynb>)

Input:
-->  'cultura_database

Output:
--> Supp Material Stats for each catalog

- [Works Stats](<../3b - stats_works.ipynb>)

Input:
-->  'cultura_database

Output:
--> Supp Material Stats for each Type of work

- [Wikipedia Creation Date Stats](<../4 - wikipedia_creation_date.ipynb>) [NOT IN THE PAPER]
- [Catalog trends](<../5 - online_catalogs_trends.ipynb>) [Figure S1]

Input:
-->  'cultura_database

Output:
--> Figure S1 of trends of different catalogs

- [text](../20-extract_works_databases.ipynb) [NOT NEEDED]
- [Single-worker versus multi-workers] Evolution of single-worker versus multi-workers

# Unseen Species Model

The unseen species model is ....

The main Ovelty is the Generalized chao estimator, but we also look at other estimators using the [copia]() packages.

For the Generalized Chao Estimator, we use a Bayesian Approach. It is advised to run the code with access to a GPU (10 minutes instead of 4 hours for the use of a L4 for instance).

Input:
    df_extract/data/
Output:
    data/unseen_species.csv
    figures/

- [Data Preprocessing](<6 NEW - preprocess_unseen_species copy.ipynb>)

Input:
    df_indi_works_occupations.csv
Output:
    unseen_species_model/individuals_into_unseen_plus_>3.csv

- [Generalized Chao](<../6c - run_best_model_north_south.ipynb>)

Input:
    unseen_species_model/individuals_into_unseen_plus_>3.csv
Output:
    unseen_species_model/unseen_species_model_bayesian.csv

- [Insights from GENERALIZED Chao](<6 GRAPH - preprocess_unseen_species.ipynb>) [FIGURE S2] [Table S4 and S5]

Input:
    unseen_species_model/unseen_species_model_bayesian.csv
    unseen_species_model/individuals_into_unseen_plus_>3.csv
Output:
    Figure and Tables

- [Estimator comparison](../estimator_robustness_analysis.ipynb)

# CPM Trends

Input:
    unseen_species_model/data/unseen_species.csv
Output:
    figures/

- [CPM_trends](<../7 - plot_region_trends.ipynb>)
- [Divergence_figures](<../8 - run_index_great_divergence.ipynb>) [Figure 1] [Figure 3] [Figure 4]
- [text](<../19 - - run_index_growth_great_divergence.ipynb>) [SUPP MATERIAL]
- Breakpoints.

# Relationships bewteen HDI, GDPpc and CPM

Input:
    unseen_species_model/data/unseen_species.csv
    environment_data/
Output:
    figures/
    data/

- [GDPpc_preprocessing](<../0 - create_gdp_data.ipynb>)
- [GDPpc_CPM](<9 - statistics_gdp_cultural_index.ipynb>) [Figure 5]
- [GDPpc_CPM](<../9b - BRM_bayesian.ipynb>) [NOT SURE IT IS USED]

## HDI

- [HDI_numeray](<../10 - numeracy.ipynb>)
- [Height](<../11 - height.ipynb>)
- [GenderEqualityofNumeracy](<../12 - - GenderEqualityofNumeracy.ipynb>)
- [CompositeMeasureofWellbeing_Compact](<../13 - CompositeMeasureofWellbeing_Compact copy.ipynb>)
- [InfantMortality_Compact](<../14 -InfantMortality_Compact.ipynb>)
- [LifeExpectancyatBirth(Total)_Compact](<../16 - -LifeExpectancyatBirth(Total)_Compact copy.ipynb>)
- [UrbanizationRatio_Compact](<../17 -UrbanizationRatio_Compact copy.ipynb>)
- [HomicideRates_Compact](<../15 -HomicideRates_Compact.xlsx.ipynb>)
- [HDI_summary_table](<../18 -HDI_summary_table.ipynb>)
- [Global]

Input:
    unseen_species_model/data/unseen_species.csv
    environment_data/
Output:
   df_indicators_hdi
