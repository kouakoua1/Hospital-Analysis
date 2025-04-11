# UK Hospital Data Analysis Project

## Introduction

This project presents an analysis of hospital data within the UK, focusing on key aspects such as hospital types, geographical distribution, sector classification (public vs. private), and organizational structures. Understanding these factors is crucial for healthcare planning, resource allocation, and gaining insights into the UK's healthcare landscape. The analysis employs data processing, statistical analysis, and visualization techniques to offer a comprehensive overview.

## Objectives

The primary objectives of this analysis were to:

* Clean and preprocess raw hospital data for quality and consistency.
* Explore the distribution of hospitals by type and subtype.
* Visualise the geographical distribution of hospitals to identify regional patterns.
* Determine the split between public (NHS Sector) and private (Independent Sector) hospitals.
* Analyse the influence of parent organizations on hospital distribution.
* Assess the completeness of hospital contact information.
* Examine the density of hospitals across latitude and longitude coordinates.

## Methodology

The analysis followed a multi-stage approach:

1.  **Data Cleaning and Preprocessing**:
    * Tool: Python (Jupyter Notebook).
    * Process: Loaded data using pandas, handled missing values, removed duplicates, and standardized formats. Columns with excessive missing data ('Address3', 'Fax,,,') were dropped. Missing categorical data was filled with 'Unknown', and numerical geographic coordinates were filled with the median. Phone and website formats were standardized. The cleaned data was saved.
2.  **Exploratory Data Analysis (EDA)**:
    * Tool: Python (Jupyter Notebook).
    * Process: Used matplotlib and seaborn for visualisations illustrating distributions of hospital types, subtypes, sector, and geographical location.
3.  **Advanced Data Analysis**:
    * Tools: Python (Jupyter Notebook) and Excel.
    * Process: Aggregated data (e.g., hospitals per city/county), calculated percentage distributions, analysed parent organization influence. Data was exported to Excel for further manipulation if needed.
4.  **Data Visualisation and Dashboarding**:
    * Tool: Power BI.
    * Process: Created interactive dashboards using key findings to provide a user-friendly interface for exploring insights.

## Analysis Highlights

* **Data Overview**: The dataset includes OrganisationID, Code, Type/SubType (mostly "Hospital"), Sector (NHS/Independent), Status, Name, Address details, Latitude/Longitude, Parent Organisation details, and Contact Information.
* **Hospital Types**: 'Hospital' is the predominant OrganisationType and SubType, indicating a focus on general hospitals. 'Mental Health Hospital' is the next most common known subtype.
* **Geographic Distribution**: Hospitals are concentrated in certain areas, particularly southern regions, with London having significantly more hospitals than other cities. A heatmap visualization showed high density in specific latitude/longitude bins, likely corresponding to major metropolitan areas, and sparser distribution elsewhere.
* **Sector Analysis**: The NHS Sector represents a larger proportion (61.4%) of hospitals compared to the Independent Sector (38.6%) in this dataset.
* **Parent Organizations**: Large parent organizations like BMI Healthcare and Spire Healthcare manage a significant number of hospitals, suggesting market consolidation.
* **Contact Information Completeness**: Website availability was excellent (100%), phone number availability was good (~79.4%), but email address availability was poor (~34.8%). All hospitals had at least one contact method listed.

## Strategic Recommendations

Based on the analysis, the following recommendations were made:

1.  **Address Geographic Disparities**: Prioritize resource allocation and potentially new facilities in underserved areas identified by the geographic analysis to improve healthcare access equity.
2.  **Enhance Data Completeness**: Implement data governance policies to improve the accuracy and completeness of contact information, especially email addresses, to facilitate communication.
3.  **Strategic Service Planning**: Tailor healthcare service planning considering the prevalence of general hospitals but also the need for specialized services like mental health.
4.  **Consider Sector Balance**: Policymakers should factor in the balance and dynamics between NHS and Independent Sector hospitals in funding and provision decisions.
5.  **Monitor Parent Organization Influence**: Regulators should monitor the impact of consolidation by large parent organizations on competition, service diversity, and patient choice.

## Conclusion

This analysis provides valuable insights into the UK hospital landscape, highlighting key trends in distribution, characteristics, and organizational structures. The findings can inform strategic decision-making in healthcare planning, resource allocation, and policy development. The combined use of Python, Excel, and Power BI enabled efficient processing and clear presentation of results.
