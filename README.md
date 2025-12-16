# A Comparative Analysis of Human Capital in African and European Economic Growth
This project was completed for QTM 302W: Technical Writing for Data Science

#### -- Project Status: Completed

## Project Intro/Objective
The purpose of this project is to analyze and compare economic growth patterns in African and European countries from 2005 to 2023, with a particular focus on the role of human capital in shaping GDP per capita. Using data from the Penn World Table, the project examines regional differences in output levels, growth rates, and the relationship between human capital, physical capital, and economic performance. By applying descriptive analysis, regression techniques, and a Cobb–Douglas production framework, the study seeks to identify structural differences in how economic inputs translate into growth across regions. The civic impact of this project lies in its potential to inform development policy by highlighting why similar levels of human capital can yield very different economic outcomes, especially in emerging economies.


### Methods Used
* Descriptive statistical analysis of GDP, GDP per capita, population, human capital, and physical capital for African and European countries (2005–2023)
* Data filtering, cleaning, and regional classification of countries using Penn World Table 11.0
* Calculation of real and PPP-adjusted GDP per capita and year-over-year growth rates
* Time-series visualization and boxplot analysis to compare regional GDP and income distributions
* Country-level growth ranking to identify fastest-growing economies by GDP per capita
* Correlation and linear regression analysis to assess the relationship between human capital and GDP per capita
* Estimation of Cobb–Douglas production functions to compare capital and human capital elasticities across regions


### Technologies
* R 
* TidyVerse
* R-markdown

## Project Description

This project examines and compares economic growth patterns in African and European countries from 2005 to 2023, with a particular focus on the role of human capital in shaping GDP per capita. Using Penn World Table (PWT) version 11.0 data, we analyze real GDP, PPP-adjusted GDP, population, employment, physical capital, and the human capital index to understand how economic inputs translate into output across regions. Because the PWT does not include regional identifiers, countries are manually grouped into Africa and Europe to enable regional aggregation and comparison.

Our analysis is guided by three main questions. First, how do GDP and GDP per capita levels and growth trends differ between African and European economies over the past two decades? Second, to what extent does human capital explain variation in GDP per capita within each region? Third, do the contributions of human and physical capital differ across regions when output is modeled using a Cobb–Douglas production framework? We hypothesize that human capital plays a more significant explanatory role in African countries, while European economic performance is less sensitive to variations in human capital alone.

To address these questions, we employ a combination of descriptive, visual, and econometric methods. We construct boxplots to compare GDP distributions over time, generate time-series plots of average GDP per capita and growth rates, and rank countries by GDP per capita growth to identify top performers. We then estimate linear regressions to assess the relationship between human capital and GDP per capita in 2023, followed by log-linear Cobb–Douglas regressions to estimate output elasticities with respect to physical and human capital for each region.

Several challenges and limitations shape the analysis. Human capital data are missing for a subset of countries, particularly smaller or less-developed economies, which requires excluding them from human-capital-specific regressions. Data sparsity in earlier years motivates restricting the sample to 2005–2023. Finally, observed gaps in GDP per capita between Africa and Europe suggest that human capital alone cannot fully explain economic performance, pointing to the influence of complementary factors such as institutions, infrastructure, and technology that fall outside the scope of the current dataset.

## Needs of This Project

* Comparable cross-country macroeconomic data
* Regional classification of countries (Africa vs Europe)
* Human capital and physical capital measures
* Cleaned and complete GDP and population data
* Tools for growth and distribution visualization
* Regression and Cobb–Douglas modeling framework
* Contextual variables for future extensions

## Getting Started

1. **Clone the repository**: Clone this repository to your local machine using Git.
2. **Locate the raw data**: All raw data files are stored in the `data/` directory, including the Penn World Table dataset (`pwt110.xlsx`) and supporting files.
3. **Run the analysis**: The main analysis is contained in `src/analysis.Rmd`. Open this file in RStudio and knit it to reproduce the results and figures.
4. **View outputs**: Rendered outputs are available in `src/analysis.html`, with intermediate LaTeX and log files also stored in the `src/` folder.
5. **Project environment**: The project is configured as an RStudio project (`QTM302W.Rproj`) to ensure consistent paths and reproducibility.

## Contributing Members
- Nate Hu
- Tristan Yang
- Tomas Hossain-Aguilar
