\# Analyzing reported issues of ZüriWieNeu 



The ZüriWieNeu online reporting platform (https://www.zueriwieneu.ch/) enables the public to report any damage or defects to Zurich's infrastructure. 



\## Objective



This Project analyses the reported issues from 2013 to 2026, regarding the temporal Evolution and spatial patterns across Zurich's neighbourhoods.



\## Data Sources



* Population data of Zurich: https://www.stadt-zuerich.ch/content/dam/web/de/politik-verwaltung/statistik-und-daten/daten/bevoelkerung/BEV321T3211\_auslaendische-Wohnbevoelkerung\_Bevoelkerung\_nach-Herkunft-Stadtkreis-Stadtquartier.xlsx
* Reported issues on ZüriWieNeu (download the .csv file for the area "Stadt Zürich"): https://www.stadt-zuerich.ch/geodaten/download/Zueri\_wie\_neu?format=10008
* Vector data of Zurich neighbourhoods (download the .gpkg file for the area "Stadt Zürich"): https://www.stadt-zuerich.ch/geodaten/download/Statistische\_Quartiere?format=10005



\## Reproducing the Environment

This project requires a specific spatial software stack. To recreate the environment

1. Ensure you have Conda installed
2. 



conda env create --name sds-env-goetz-copy --file sds-env-goetz.yml



Use a conda environment with packages similar to ...



Open Jupyter Lab from in your environment

