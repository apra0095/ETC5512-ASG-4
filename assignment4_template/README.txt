### Description of Data Origin
- FAO Prevalence of Undernourishment Index which estimates the share of a nation’s population falling below a 
minimum daily calorie requirement based on national food‐supply records and household surveys.
- OECD PISA Scores in Science, Math, and Reading, which sample 15-year-old students every 
three years to assess real-world problem-solving skills across countries.

### Description of The Files Included
-data/fao_data.csv
 -Tidy FAO data with one row per country and year (2009–2022), containing:
  -country_name
  -year
  -undernourishment_pct

-data/pisa_science.csv, pisa_math.csv, pisa_reading.csv
 -Each file holds score for specific asessment of science, math, and reading with:
  -country
  -year (2009, 2012, 2015, 2018, 2022)
  
### Author and Date of Release
-Author: Izzul Fattah Aji Pratama
-Date of Release: 18 Jun 2025

### Description of How to Use The Data
These processed CSVs are ready for analysis in R, 
or any environment that can read comma-separated values. They combine undernourishment rates with PISA domain scores 
.Both numeric (percentages, scores) and categorical (country names) fields are present—refer to each file’s header row for 
column names. User could refer to **Data Dictionary** for detailed description.

### Relevant Assumptions
-Modelled estimates: FAO’s undernourishment rates are statistical estimates, not direct counts. 
When food‐supply or survey data are missing or delayed, the model fills in the gap.
-Sample survey limitations: PISA scores come from a sample of 15-year-olds. 
some countries may have missing values where participation fell below thresholds.
-Data alignment: Country names have been cleaned (e.g. removed “(2015)” suffixes)