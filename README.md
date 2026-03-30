# COVID-19 Data Analysis & Dashboard

## Overview
This project analyzes global COVID-19 trends using SQL and Tableau to uncover insights related to infection rates, death rates, and vaccination progress across countries and continents. The goal is to transform raw pandemic data into meaningful insights that highlight patterns in public health outcomes.

---

## Data Sources and Tools

**Data Sources**
- COVID-19 Deaths Dataset (Excel)
- COVID-19 Vaccinations Dataset (Excel)

**Tools Used**
- SQL (MySQL) – data cleaning, transformation, and analysis  
- Tableau – interactive dashboard visualization  
- Excel – initial data storage and formatting  

---

## Key Questions Answered

- What is the likelihood of death after contracting COVID-19 in different countries?
- What percentage of a country’s population was infected?
- Which countries had the highest infection rates relative to population?
- Which countries and continents had the highest death counts?
- What are the global totals for cases, deaths, and death percentage?
- How did vaccination rollout progress over time across countries?
- What percentage of populations were vaccinated over time?

---

## Visual Overview

The Tableau dashboard provides:
- Global trends in COVID-19 cases and deaths
- Country-level comparisons of infection and death rates
- Vaccination progress over time using rolling totals
- Continent-level summaries for high-level insights

---

## Technical Workflow Summary

1. **Database Creation**
   - Created structured tables for deaths and vaccinations data
   - Defined appropriate data types for metrics such as cases, deaths, and population

2. **Data Exploration**
   - Filtered relevant records (excluding null continents)
   - Analyzed relationships between total cases, deaths, and population

3. **Key Calculations**
   - Death percentage:
     - `(total_deaths / total_cases) * 100`
   - Infection rate:
     - `(total_cases / population) * 100`

4. **Aggregations**
   - Identified highest infection rates by country
   - Calculated total deaths by country and continent
   - Computed global totals for cases and deaths

5. **Advanced SQL Techniques**
   - Window functions for rolling vaccination totals
   - Common Table Expressions (CTEs) for structured analysis
   - Temporary tables for intermediate calculations
   - Views created for reusable analysis and Tableau integration

6. **Data Integration**
   - Joined deaths and vaccination datasets on location and date
   - Built rolling vaccination metrics to track progress over time

7. **Visualization**
   - Connected SQL outputs to Tableau
   - Designed dashboard to highlight key trends and comparisons

---

## Files Included

- `Covid Queries.sql` – SQL queries for data cleaning, analysis, and view creation :contentReference[oaicite:0]{index=0}  
- `CovidDeaths.xlsx` – dataset containing COVID-19 cases and deaths  
- `CovidVaccinations.xlsx` – dataset containing vaccination and testing data  
- `Covid Dashboard.twb` – Tableau dashboard file for visualization  

---

## Key Insights

- Infection and death rates varied significantly across countries
- Larger populations did not always correlate with higher infection percentages
- Vaccination rollouts showed strong variation in speed and coverage
- Rolling vaccination metrics provided a clearer picture of progress over time
- Global death percentage highlighted the overall severity of the pandemic

---

## Future Improvements

- Add predictive modeling for case trends
- Incorporate more recent or real-time COVID-19 data
- Enhance dashboard interactivity with filters and drill-downs
- Deploy dashboard publicly for easier access

---
