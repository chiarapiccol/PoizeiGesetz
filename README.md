# PoizeiGesetz Analysis
This repository contains the analysis for the the seminar project "Poizeigesetz Analysis" by Dr. Sebastian Köhler. The analysis focuses on the data from the BKA and GESIS datasets to understand various aspects related to policy reforms, crime statistics, and socioeconomic factors.

## 1. Packages
The following R packages are required: 
tidyverse
haven
dplyr
readxl
plyr
ggplot2
reshape2
stringi
Synth

## 2. Data Import and Adjustment
This section involves importing and adjusting data tables from BKA and GESIS to create dataframes:

- Import BKA tables for the years 2013-2020.
- Adjust the tables to add a "Jahr" column and standardize "Bundesland" names.
- Merge BKA tables into a single dataframe "LF" for descriptive statistics.
- Adjust the merged dataframe to create new variables and regroup crime categories.
- Import and adjust additional SO tables.
- Merge SO tables into a dataframe "SO" for analysis.
- Create new variables in the dataframe "SO" for various socioeconomic indicators.
- Save the adjusted dataframes for further analysis.

## 3. Descriptive Statistics
In this section, the dataframes LF and LSO are used to provide an overview of the data:

- Development over time and across different Länder.
- Analysis of the development of crime rates categorized by different crime groups.
- Visualization of the trends using ggplot2.

## 4. Analysis
This section combines the SO and BKA dataframes for analysis and hypothesis testing:

- Adjust the dataframe to fit the analysis criteria.
- Use Synthetic Control Methods to analyze the impact of policy reforms on crime rates.
- Prepare the data for the synth() function to conduct comparative case studies.
- Generate plots and tables to visualize the results and gaps.
