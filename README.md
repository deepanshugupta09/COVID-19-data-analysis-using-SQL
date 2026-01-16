# COVID-19 Data Analysis using SQL

## Project Overview
This project analyzes COVID-19 data using SQL to extract insights related to cases, deaths, and vaccinations.

## Dataset
- Source: Our World in Data
- Tables Used:
  - covid_deaths
  - covid_vaccinations

## Tools Used
- PostgreSQL
- SQL
- GitHub

## Key Analysis
- Looking For Total_Cases Vs Total_deaths
- Looking At Total_Cases Vs Total_Population
- Shows What Percentage Of Population Get Covid
- Looking  At Countries With Highest Infection Rate Compared To Population.
- Showing Countries With Highest Death Count Per Population
- Let's Break Things Down By Continent
- Showing Contintents with the highest deaths count per population
- Global Numbers
- Looking total population vs vaccinations
- Temp Table
- Creating View To Store Data For Latter Visualizations

## Sample Query
```sql
SELECT location, date, total_cases, total_deaths,
       (total_deaths / total_cases) * 100 AS death_percentage
FROM covid_deaths;
