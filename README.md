# Brownfield Redevelopment Tax Credit Analysis (New York State)

## Project Overview

This project analyses **New York State Brownfield Redevelopment Tax Credit (BRTC)** data to understand the policy impact in New York City from the time the policy was implemented till 2024 (does the program improve the number of brownfields developed annually in New York City(2007-2024)?.  I explored how redevelopment costs, environmental zones, geographic regions, and project types influence tax credits awarded. The aim is to provide **descriptive, environmental, spatial, and financial insights** that support evidence‑based policy evaluation and investment decision‑making.

---

## Objectives

* Examine **trends in brownfield projects over time**
* Analyse **cost vs. credit relationships**
* Identify **top developers/taxpayers** by project count and credit received
* Compare **Environmental Zone vs Non‑Environmental Zone** projects
* Assess **regional disparities** across DEC regions
* Visualise **spatial distribution** of brownfield sites
* Evaluate **financial efficiency** of redevelopment spending

---

## Data Source

* **Dataset**: New York State Brownfield Redevelopment Credit – Beginning Calendar Year
* **Publisher**: NYS Open Data
* **Access Method**: Public Google Drive link (used for reproducibility and ease of access)
* **Geographic Coverage**: New York State

### Key Variables

* Calendar Year
* Project Site Code
* Developer / Taxpayer
* Total Redevelopment Cost
* Tax Credit Awarded
* Environmental Zone Indicator
* DEC Region
* Project Type
* Georeference (Latitude / Longitude)

> **Assumptions to fix missing values**:
> * Since calculation of credit requires complex calculation and tax professional oversight, it was assumed that most credits awarded represent approximately half of incurred redevelopment costs
> * Projects sharing the same site code also share the same georeference, therefroe missing georeferences were inferred using project site codes where applicable

---

## Tools & Technologies

* **Python**: Data cleaning, transformation, and exploratory analysis
* **Jupyter Notebook**: Main analysis workflow
* **Pandas / NumPy**: Data manipulation
* **Matplotlib / Seaborn**: Visualisation
* **Tableau**: Interactive dashboards and spatial analysis (`Assess.twbx`)

---

## Repository Structure

```
├── DAS7000_st20337247.ipynb   # Main analysis notebook
├── Assess.twbx               # Tableau dashboard and spatial visualisations
├── README.md                 # Project documentation
```

---

## Analysis Summary

### 1. Descriptive Analysis

* Brownfield projects show a **steady annual increase**, indicating growing participation in redevelopment incentives.
* Redevelopment cost and awarded credits are positively correlated but vary across regions and project types.

### 2. Environmental & Spatial Analysis

* Approximately **55% of projects are located in Environmental Zones**.
* **New York City DEC Region** accounts for the largest share of projects and credits.
* Spatial mapping highlights clustering in historically industrialised regions.

### 3. Financial Analysis

* Large‑scale projects dominate total redevelopment costs and credits.
* Regional differences suggest **uneven redevelopment efficiency** across the state.
* Higher cost‑credit ratios in some regions may reflect contamination complexity.

---

## Key Insights

* Brownfield incentives effectively stimulate redevelopment but show **regional imbalance**.
* Environmental Zones attract slightly more projects, reflecting targeted policy success.
* Financial outcomes vary significantly by DEC region and project scale.

---

## How to Run the Project

1. Clone the repository

```bash
git clone https://github.com/Medynal/Pollution.git
```

2. Open the Jupyter Notebook

```bash
jupyter notebook DAS7000_st20337247.ipynb
```

3. (Optional) Open `Assess.twbx` in Tableau Desktop for interactive visualisations

---

## Limitations
* Financial figures are nominal (not inflation‑adjusted)
* Some geospatial data required assumptions due to missing values
* Analysis is descriptive; no causal inference is established


---

## Future Work

* Apply **regression or machine learning models** to predict credit allocation
* Perform **inflation‑adjusted financial analysis**
* Extend spatial analysis with socioeconomic indicators
* Compare New York outcomes with other US states

---

## Author

**Modinat Adeyemi**
MSc Data Science – Cardiff Metropolitan University

---

## Licence

This project is for academic use. Data ownership remains with NYS Open Data.
