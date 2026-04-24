# Chicago Tax Increment Financing (TIF) Analysis

## Overview

Tax Increment Financing (TIF) is a public financing tool used by municipalities to encourage economic development in designated areas. In Chicago, TIF districts redirect incremental property tax revenue generated within defined boundaries toward local development projects.

This project analyzes TIF districts in Chicago, focusing on their spatial distribution and their relationship with changes in property values and municipal tax levies over time.

---

## Project Context

This project was originally started during my internship with the Cook County Assessor’s Office (CCAO) from Jan 2026 to Mar 2026. After the internship concluded, I continued developing and extending the analysis independently.

This repository reflects my own work and extensions of the original project. It is not an official work product of the Cook County Assessor’s Office and has not been reviewed or endorsed by CCAO.

---
## View memo [here!](https://rushikeshay.github.io/tif-districts-analysis-ccao-project/) 
## Objectives

- Analyze spatial distribution of TIF districts in Chicago  
- Explore changes in property values within and outside TIF areas  
- Assess fiscal implications of TIF surplus allocation  
- Build reproducible geospatial and statistical workflows  

---

## Package Dependencies

```r
library(data.table)
library(glue)
library(here)
library(DBI)
library(RSQLite)
library(ptaxsim)
library(vctrs)
library(dplyr)
library(tidyverse)
library(httr)
library(jsonlite)
library(ccao)
library(ggplot2)
library(plotly)
library(statip)
library(scales)
library(crosstalk)
library(htmltools)
library(sf)
library(ggspatial)
library(prettymapr)
library(purrr)
library(RColorBrewer)
```
## Key Methods

- Geospatial analysis using `sf`  
- Data wrangling with `dplyr` and `data.table`  
- Interactive visualization with `plotly`  
- Spatial mapping with `ggspatial`  
- Property tax data processing using `ptaxsim`  
- API ingestion using `httr` and `jsonlite`  

---

## Key Outputs

### TIF Concentration
- Share of PINs within TIF districts by municipality  
- Identification of high TIF-penetration municipalities  

### Property Value Dynamics
- Time series of total EAV vs frozen base  
- TIF increment growth across municipalities  
- Cross-city comparison (Phoenix, Bedford Park, Bellwood, Ford Heights, Posen)  

### Effective Tax Rates
- Actual vs counterfactual tax rates  
- Estimated rate inflation due to TIF base reduction  
- Agency-level decomposition (school, municipal, park districts)  

---

## Author

Rushikesh Jadhav
