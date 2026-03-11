# Maji-Ndogo-Agricultural-Data-Automation
A modular Python data pipeline for agricultural analysis. Integrates SQL relational data, performs automated ETL/data cleaning, and identifies optimal crop-growth conditions through functional programming.

- Project Scope: Maji Ndogo Data-Automation

Overview: The Maji Ndogo Data-Automation project is a data engineering and analytical study designed to optimize crop production in a developing region. The scope of this project covers the entire data lifecycle—from extracting raw, siloed data out of a relational database to providing high-level strategic recommendations for agricultural deployment. The project simulates the role of a Data Scientist/Engineer tasked with determining where the region's limited resources (automated farming technology) should be deployed to maximize yield and sustainability.

- Project Objectives: Data Integration (Extraction)The initial scope involves breaking down data silos. Agricultural information was spread across four distinct database tables. This project implements a unified data structure by joining

A, Geographic Data

B, Field locations

C, Physical Terrain Features

- Weather Patterns: Historical rainfall and temperature data
Soil Characteristics: Chemical composition and fertility scores
Management Records: Crop types and historical yield performance

- Data Quality & ETL (Transformation)A major component of this project is identifying and programmatically fixing "dirty data." The scope includes;

1, Schema Correction: Resolving a critical error where column headers (Crop_type and Annual_yield) were inverted.

2, String Standardization: Cleaning categorical data to remove "fuzzy" duplicates and spelling errors (e.g., standardizing 'teaa' to 'tea').

3, Range Validation: Correcting geographic outliers, such as negative elevation values, to ensure geospatial accuracy.

- Environmental Analysis (Insight)The project identifies the "environmental signature" of Maji Ndogo's crops. By analyzing the relationship between geography and biology, the project determines hich soil types (e.g., Silt, Volcanic) provide a natural competitive advantage. The optimal elevation and rainfall "sweet spots" for high-value crops like Tea and Wheat. 

- Strategic Recommendation (Final Output)The ultimate goal is to isolate High-Potential Fields. The project filters the master dataset to find specific plots of land that meet a "Perfect Condition" profile. Above-average historical yield, Optimal temperature windows ($12^{\circ}C$ - $15^{\circ}C$), & Zero to low pollution levels.

- Tech Stack - SQL & SQLAlchemy: For relational database management and 4-way table joins.
Python (Pandas & NumPy): For data manipulation, cleaning, and statistical aggregation.

Matplotlib: For visualizing trends in soil fertility and yield distribution.

Modular Programming: Refactoring logic into independent scripts for Ingestion, Cleaning, and Analysis.

- Expected Outcomes: By the end of this project, we move from a messy, unreliable database to a prioritized list of high-yield fields. This allows the government or NGO stakeholders to move from "guesswork" to "data-driven" agricultural management, ensuring that technology is only deployed where it has the highest probability of success.
