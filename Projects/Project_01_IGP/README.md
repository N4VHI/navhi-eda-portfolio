![Status](https://img.shields.io/badge/status-completed-brightgreen)
![Python](https://img.shields.io/badge/python-3.x-blue)
![EDA](https://img.shields.io/badge/type-EDA-orange)

# Peruvian Earthquake Behavior Analysis (1960–2025)

## Background
Peru lies within the Pacific Ring of Fire, making it one of the most seismically active regions in the world.  
This project analyzes historical earthquake records to explore spatial distribution, temporal patterns, and relationships between key earthquake characteristics such as depth and magnitude.

---

## Objectives
- Identify temporal trends in earthquake occurrences over time
- Detect geographic regions with higher seismic activity
- Explore relationships between earthquake depth, magnitude, and location
- Understand potential biases in historical earthquake recording

---

## Data Sources

### Earthquake Records
- IGP Historical Earthquake Repository  
  https://ultimosismo.igp.gob.pe/repositorio/datos-sismicos

**Reproducibility**
1. Download the Excel dataset
2. Rename it to: `datos-sismicos.xlsx`
3. Place it inside: `data/raw/`

---

### Geographic Data

**Peru Department Boundaries (Shapefile)**  
https://www.datosabiertos.gob.pe/dataset/limites-departamentales

**Peru Geographic Regions (Shapefile)**  
https://peru.mapbiomas.org/en/capas/

**World Oceans (Shapefile)**  
https://techgeo.org/download-world-oceans-in-shapefile-geojson-and-kml-format/

Reproducibility:
- Extract the shapefiles
- Copy the folders into `data/raw/`

---

## Project Structure

```

project/
│
├── notebooks/
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_cleaning.ipynb
│   ├── 03_univariate_analysis.ipynb
│   └── 04_multivariate_analysis.ipynb
│
├── reports/
│   └── figures/
│
├── data/
│   └── raw/
│   └── processed/
│
└── 05_key_findings.md

```

---

## Process
1. **Data Understanding**
   - Initial exploration of variables and structure
   - Identification of missing values and inconsistencies

2. **Data Cleaning**
   - Datetime standardization
   - Column normalization
   - Handling missing or inconsistent records

3. **Univariate Analysis**
   - Distribution of magnitudes and depths
   - Earthquake counts by year, day, and time
   - Geographic frequency by department and region

4. **Multivariate Analysis**
   - Correlation analysis
   - Depth vs magnitude exploration
   - Spatial relationships

5. **Key Findings & Reporting**
   - Executive summary
   - Visual storytelling
   - Interpretation of trends

---

## Key Insights
- No strong correlation was found between earthquake depth and magnitude.
- The apparent increase in earthquake frequency over recent decades is likely influenced by improvements in seismic monitoring technology rather than a true increase in seismic events.
- Most earthquakes occur at shallow depths.
- A significant number of events occur offshore along the Pacific Ocean due to tectonic subduction processes.

---

## Tools & Technologies
- Python
- Pandas
- NumPy
- Seaborn & Matplotlib
- GeoPandas
- Jupyter Notebook
- Git & GitHub

---

## Author
Data analysis portfolio project focused on exploratory data analysis (EDA) and geospatial investigation.