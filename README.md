# covid_19_Data_Analysis


# Project Plan


The data for this project was collected from the research titled "Coronavirus Pandemic (COVID-19)" published online at Our World in Data. We can get the data from the Coronavirus Pandemic (COVID-19) - Statistics and Research - Our World in Data. The primary data source for the Confirmed and death cases is the COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University. The data for Policy responses was obtained from Oxford COVID-10 Government Response Tracker. The data for Vaccinations, Tests and positivity, Hospitals and ICU is obtained from the Official data collected by the OurWorld in data team. The confirmed cases and the deaths data is updated daily. The dataset contains the Covid-19 information about almost all the countries in the world. 

 The dataset contains the following variables:
 
1. location : country name
2. date : date on which the observation was made
3. total_cases : total cases of COVID-19 till date
4. new_cases :  COVID-19 cases recorded on the particular date
5. total_cases_per_million : Total confirmed cases of COVID-19 per 1,000,000 people.
6. total_deaths : Total deaths attributed to COVID-19 till date
7. new_deaths : New deaths attributed to COVID-19 on a specific date
8. new_tests : New tests conducted on a given date
9. total_tests : total tests done till date
10. new_tests_per_thousand : new tests done on a particular date per thousand population
11. total_tests_per_thousand : total tests done on a particular date per thousand population
12. hosp_patients : Number of COVID-19 patients in hospital on a given day
13. new_vaccinations : New COVID-19 vaccination doses administered
14. people_vaccinated : Total number of people who received at least one vaccine dose




## Project Aim and Objectives 

The project aims to analyse the trend of the COVID-19 globally. Live data is used for this project.  The data is available from March 2021 to date.  We would show the map view of the world to show the countries affected by the COVID-19 and the spread of the infection. We would also try to study the impact of COVID-19 lockdown interventions in different countries on the spread of COVID-19 cases and the deaths due to COVID-19. After mapping the 5 top countries that are effected by the COVID-19, for ease of analysis and understanding, we choose the top five countries to analyse and visualise the impact of lockdown restrictions. We also study the relation between the COVID-19 positivity rate and the number of tests conducted.

### Specific Objective(s)

* __Objective 1:__ Analyse and Visualise the impact of COVID-19 Lockdown measures on the spread of COVID-19 infection - whether the infection rate increased or decreased.
* __Objective 2:__ Total COVID-19 tests conducted vs confirmed cases.
* __Objective 3:__ Visualise and analyse the impact of COVID vaccination on the hospitilisation of infected patients.


## System Design


### Architecture

The data is collected from a URL as a single CSV file from "Our World in Data" repository. First, the cleaning process is performed where the unwanted rows and columns are dropped. Cleaned data is then used to plot a world map with the choropleth world maps for visualisation. Then the data is grouped and filtered by countries and dates to perform the Exploratory Data Analysis and the analysis objectives are explained and visualised in the following sections.
  
### Processing Modules and Algorithms

* Data cleaning - We obtined the data from https://ourworldindata.org/coronavirus. The dataset was cleaned by dropping the unwanted rows and columns and the analysis was carried forward to only top countries effected by the COVID-19. In case of Missing values the data was made clean and easy to analyse.
* Dataset was filtered  and visualised using plotly.
