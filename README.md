# Analyzing Reported Issues of ZüriWieNeu

The ZüriWieNeu online reporting platform (https://www.zueriwieneu.ch/) enables the public to report damage or defects in Zurich's public infrastructure.

## Objective

This project analyses reported issues from 2013 to 2026, focusing on their temporal evolution and spatial patterns across Zurich's neighbourhoods.

## Data Sources

The raw data files are not included in this repository and must be downloaded manually.

### Population data of Zurich

Download the Excel file:

https://www.stadt-zuerich.ch/content/dam/web/de/politik-verwaltung/statistik-und-daten/daten/bevoelkerung/BEV321T3211_auslaendische-Wohnbevoelkerung_Bevoelkerung_nach-Herkunft-Stadtkreis-Stadtquartier.xlsx

### Reported issues on ZüriWieNeu

Download the `.csv` file for the area **Stadt Zürich**:

https://www.stadt-zuerich.ch/geodaten/download/Zueri_wie_neu?format=10008

### Vector data of Zurich neighbourhoods

Download the `.gpkg` file for the area **Stadt Zürich**:

https://www.stadt-zuerich.ch/geodaten/download/Statistische_Quartiere?format=10005

## Reproducing the Environment

This project requires a spatial Python environment. To recreate the environment:

### 1. Ensure that Conda is installed

You can use either Anaconda or Miniconda.

### 2. Clone this repository

```bash
git clone https://github.com/lukasgoetz-debug/sds210-project-lukas-goetz.git
```

### 3. Navigate to the project folder

```bash
cd sds210-project-lukas-goetz
```

### 4. Create the Conda environment from the YAML file

```bash
conda env create --file sds-env-goetz.yml
```

### 5. Activate the environment

```bash
conda activate sds-env-goetz
```

## Running the Analysis

After activating the environment:

### 1. Download the raw data

Download the three raw data files from the links listed in the **Data Sources** section.

### 2. Store the downloaded files

Place all downloaded raw files in:

```text
data/raw/
```

### 3. Open JupyterLab from the project folder

```bash
jupyter lab
```

### 4. Open the notebooks

Open the notebooks in the `notebooks/` folder.

### 5. Run the notebooks in this order

1. `notebooks/01_zwn_data.ipynb`
2. `notebooks/02_pop_quartiere_data.ipynb`
3. `notebooks/03_analysis_plots.ipynb`

### 6. Outputs

Generated cleaned datasets are stored in:

```text
data/cleaned/
```

Generated plots, figures, and maps are stored in:

```text
outputs/
```

## Project Structure

The project is organised as follows:

```text
sds210-project-lukas-goetz/
│
├── data/
│   ├── raw/          # Original downloaded data files
│   └── cleaned/      # Cleaned data created during preprocessing
│
├── notebooks/
│   ├── 01_zwn_data.ipynb
│   ├── 02_pop_quartiere_data.ipynb
│   └── 03_analysis_plots.ipynb
│
├── outputs/          # Saved figures and maps
│
├── sds-env-goetz.yml # Conda environment file
├── .gitignore
└── README.md
```

## Notes

The folders `data/raw/`, `data/cleaned/`, and `outputs/` are included in the repository using `.gitkeep` placeholder files.

However, the actual raw data, cleaned data, and generated outputs are ignored by Git and are therefore not uploaded to GitHub.

This keeps the repository lightweight and avoids committing large or generated files.