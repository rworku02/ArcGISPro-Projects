# Mapping Poverty and Data Uncertainty in King County

This project analyzed the distribution of residents living below 150% of the federal poverty level across King County census tracts using data from the CDC Social Vulnerability Index (SVI) and the American Community Survey (ACS). Beyond mapping poverty counts and percentages, the analysis focused on measuring and visualizing uncertainty using margins of error (MOE) and coefficients of variation (CV). The work highlights how data reliability affects interpretation and policy targeting for organizations addressing food insecurity and poverty.


The primary goal of this project was to gain practical experience integrating ACS data into ArcGIS workflows while emphasizing the importance of mapping statistical uncertainty. The project included:

1. Downloading and processing ACS/CDC SVI data at the census tract level.

2. Mapping poverty counts, MOEs, and CVs to evaluate estimate reliability.

3. Using the ACS Statistical Toolkit in ArcGIS to derive percentage-based poverty measures and calculate associated error margins.

4. Producing policy-relevant layouts and a report for a nonprofit partner (Food Lifeline) to inform resource allocation strategies in King County.

## Skills Gained

- Data acquisition from ACS (Census Bureau) and CDC SVI portal

- Spatial data preprocessing: subsetting Washington census tract shapefiles to King County

- Uncertainty quantification: manual CV calculation (MOE/1.645/Estimate) and interpretation using reliability thresholds (high, medium, low)

- Application of the ACS Statistical Toolbox in ArcGIS Pro (Derived Proportion MOE, CV Calculator, Statistical Difference tools)

- Cartographic design: side-by-side layouts of estimates and reliability for direct comparison

- Translation of technical analysis into policy-relevant reporting for nonprofits addressing poverty

## Tools & Data

ArcGIS Pro: spatial analysis, ACS statistical toolbox, map layouts

CDC Social Vulnerability Index (2022): prepared ACS estimates and margins of error

TIGER/Line Shapefiles: Census tract boundaries for King County, WA

U.S. Census Bureau ACS (2018–2022, 5-year estimates)

## Key Insights

Highest poverty concentrations were identified in South Seattle and select tracts in South King County. CV analysis revealed that areas with the largest impoverished populations also had wide margins of error, highlighting the importance of incorporating reliability before drawing conclusions. When shifting from counts to percentages of population below 150% poverty, a different spatial pattern emerged — rural tracts had higher poverty rates despite smaller populations. The ACS Statistical Toolbox streamlined the calculation of derived MOEs and CVs, making it possible to present a nuanced landscape of both poverty distribution and estimate reliability.

Final outputs included maps and a report for Food Lifeline, guiding decisions on which census tracts should be prioritized for food security interventions given both population need and data reliability.

<img width="792" height="612" alt="image" src="https://github.com/user-attachments/assets/bac41ea3-8420-4b1b-b5c1-5e8884874ce5" />


