# COVID19_Project

## Final Slide-Deck of Results
 * COVID19_Project | Spring 2020  

## Individual Jupyter Notebook EDA Files
Files created individually for EDA of COVID19 data.
 * covid_eda_augsburger-v2.ipynb
 * covid_eda_lee.ipynb
 * covid_eda_nusaputra.ipynb
 * covid_eda_sawasaki.ipynb

## Data
* data_pkl: data sets that were pickled
* data_processing: jupyter notebook files of processing raw data to usable datasets.
* data_raw: raw dataset from sources that were saved
* data_sourcing: data cleaning raw data

## Miscellaneous
* miscellaneous: files needed for geopandas package and animation plots created from EDA

## Data Sources Findings

We sources 3 versions of COVID-19 from the following sources: 

1. New York Times COVID-19 Github repository: https://github.com/nytimes/covid-19-data 

  **We recommend not using this source, as the sources below seemed to have a more ideal format**
  
  * Advantages: 
    * Already in long format, at the state and county level
  * Disadvantages:
    * Mix of county versus city level data, so many FIPS codes are missing 
    * The way data are updated makes it unclear why there are discrepancies in cases/deaths for each date for a given location, and thus which count should be used

2. USA Facts: https://usafacts.org/visualizations/coronavirus-covid-19-spread-map/

  **We recommend using this source for county-level COVID analyses**

  * Advantages:
    * County-level COVID cases, deaths, and overall population data are well documented with clean FIPS codes. These can be merged together and on other data sources.
  * Disadvantages: 
    * In wide format with columns for every date, which means that it must be transformed to long format for most analyses

3. COVID Tracking Project: https://covidtracking.com/data

  **We recommend using this source for state-level COVID analyses**

  * Advantages:
    * Very detailed COVID data, including information about what treatments people are getting (e.g., how many people are in ICU) 
    * Clean FIPS codes can be merged on other data.
  * Disadvantages:
    * Only at the state level 
    
## How to use this repo

* If you are interested in sourcing the most up-to-date data yourself or in our documentation of different sources, you can use our sourcing scripts in the data_sourcing folder (see above for guidelines on which to use)
* If you are interested in using the COVID-19 data we downloaded and processed, you can use the files in the the Data_pkl/covid19 folder. Here is an article on how to read in this type of data to Python: https://wiki.python.org/moin/UsingPickle 
* If you are interested in our exploratory findings, you can look through our Jupyter Notebook EDA files
* Please fork/use this repo, and start an issue to collaborate with us! We are always looking to improve and would like to hear from you.



