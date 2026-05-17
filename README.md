\# Analyzing Reported Issues of ZüriWieNeu



The ZüriWieNeu online reporting platform (https://www.zueriwieneu.ch/) enables the public to report damage or defects in Zurich's public infrastructure.



\## Objective



This project analyses reported issues from 2013 to 2026, focusing on their temporal evolution and spatial patterns across Zurich's neighbourhoods.



\## Data Sources



\- Population data of Zurich:  

&#x20; https://www.stadt-zuerich.ch/content/dam/web/de/politik-verwaltung/statistik-und-daten/daten/bevoelkerung/BEV321T3211\_auslaendische-Wohnbevoelkerung\_Bevoelkerung\_nach-Herkunft-Stadtkreis-Stadtquartier.xlsx



\- Reported issues on ZüriWieNeu:  

&#x20; Download the `.csv` file for the area \*\*Stadt Zürich\*\*:  

&#x20; https://www.stadt-zuerich.ch/geodaten/download/Zueri\_wie\_neu?format=10008



\- Vector data of Zurich neighbourhoods:  

&#x20; Download the `.gpkg` file for the area \*\*Stadt Zürich\*\*:  

&#x20; https://www.stadt-zuerich.ch/geodaten/download/Statistische\_Quartiere?format=10005



\## Reproducing the Environment



This project requires a spatial Python environment. To recreate the environment:



1\. Ensure that Conda is installed.



2\. Clone this repository:



&#x20;  ```bash

&#x20;  git clone https://github.com/lukasgoetz-debug/sds210-project-lukas-goetz.git

&#x20;  ```



3\. Navigate to the project folder:



&#x20;  ```bash

&#x20;  cd sds210-project-lukas-goetz

&#x20;  ```



4\. Create the Conda environment from the YAML file:



&#x20;  ```bash

&#x20;  conda env create --file sds-env-goetz.yml

&#x20;  ```



5\. Activate the environment:



&#x20;  ```bash

&#x20;  conda activate sds-env-goetz

&#x20;  ```



\## Running the Analysis



After activating the environment:



1\. Download the raw data from the links above.



2\. Store the downloaded files in the `data/raw/` folder.



3\. Open JupyterLab from the project folder:



&#x20;  ```bash

&#x20;  jupyter lab

&#x20;  ```



4\. Open the notebooks in the `notebooks/` folder.



5\. Run the notebooks in this order:



&#x20;  1. `notebooks/01\_zwn\_data.ipynb`

&#x20;  2. `notebooks/02\_pop\_quartiere\_data.ipynb`

&#x20;  3. `notebooks/03\_analysis\_plots.ipynb`



6\. All generated plots are automatically stored in the `outputs/` folder.



\## Project Structure



The project is organised as follows:



```text

sds210-project-lukas-goetz/

│

├── data/

│   ├── raw/          # Original downloaded data files

│   └── cleaned/      # Cleaned data created during preprocessing

│

├── notebooks/

│   ├── 01\_zwn\_data.ipynb

│   ├── 02\_pop\_quartiere\_data.ipynb

│   └── 03\_analysis\_plots.ipynb

│

├── outputs/          # Saved figures and maps

│

├── sds-env-goetz.yml

└── README.md

```

