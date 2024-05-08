# Ying's-Data-Science-Profile
Project Demo

# Deep Learning Project
# [Malaria Detection Using AI-based tool (CNN-by-tensorflow)]

## Introduction 
The traditional manual microscopic diagnosis is time-consuming and test results vary among observers. This project proposed a AI-based malaria detection model leveraging Convolutional Neural Networks (CNNs) to accurately identify malaria parasites (with accuracy of 98.4%) in blood smear miscroscopic images. 

The key questions for this project is to answer:
1) Can a CNN-based ML model detect parasite in red blood cells?
2) How accurately the CNN model can classify malaria infected and uninfected red blood cells?
3) How to implement the AI-based solution to streamline the malaria detection?
4) How the AI-based solution help monitoring Malaria prevalence?


The detected blood cell images are preprossed by HSV-transformed with Gaussian blurring, which reduce the image noise and enhance the capabilities of differentiating parasites from cell impurities under different microscopic lighting conditions. The proposed final CNN model is improved with LeakyReLU and Batch Normalization. 

### Data Description
There are a total of 24,958 train images and 2,600 test images (colored) m microscopic images. These images are of the following categories:

Parasitized: The parasitized cells contain the Plasmodium parasite which causes malaria (12582 cell images in training set, and 1300 cell images in test set)
Uninfected: The uninfected cells are free of the Plasmodium parasites (12376 cell images in training set, and 1300 cell images in test set)

Acknowledgements: This dataset was taken from the National Institutes of Health (NIH) website (https://www.nih.gov/, accessed on 11 August 2022) and contains 27,558 photos, including 15,376 uninfected cell images and 15,582 infected cell images.


# Python Project 1
# [Covid19 Python Dashboard (Data Science MA705 Individual Final Project)](https://ma705covid19-project.herokuapp.com/)


The final dashboard of "Realtime Covid-19 Cases and Vaccinations in Most Populous States in the United States" is deployed on Heroku [Click here](https://ma705covid19-project.herokuapp.com/)

For the details and Python code, please check out [Here: Python Code ](https://github.com/hattie913/ma705-Project-PythonDashboard)

## Dashboard Description

The dashboard demonstrates how Covid-19 cases and new doses of vaccinations implemented daily in some populous US states change over time since the vaccine began to deployed nationwide in January 2021. The dashboard collects real-time data in Massachusetts and the other top 10 most populated states in the US.

Users can compare and overview the change of vcaccination implementations and daily counts of Covid-19 cases across those big states on the real-time, interactive time series graph, and get more detailed information on the table at the bottom.

### Data Sources

Data from this dashboard was collected from [Centers for Disease Control and Prevention](https://covid.cdc.gov/covid-data-tracker/#cases_casesper100klast7days), and [Our World in Data](https://ourworldindata.org/us-states-vaccinations).

- Source of Covid-19 cases dataset: [Covid-19 cases from SODA API endpoint](https://data.cdc.gov/resource/9mfq-cb36.json)
- Source of US vaccination dataset: [US Vaccinations](https://github.com/owid/covid-19-data/tree/master/public/data/vaccinations)

The 'realtime_Covid.py' file generates the target dataset for analyzing. The raw datasets were first cleaned by dropping unnecessary rows of states and columns of variables, and filling missing values with 0s. Before merging the two datasets, the Covid-19 cases dataset was also cleaned by grouping 'NY' and 'NYC'on the same date and then add the aggregated daily data of the entire New York State to the original dataset. Having the identical state abbreviation, the two datasets were then merged on their state abbreviation and date, then the merged dataset was saved as a 'pkl' file for the downstream analysis. 


### Variable Interpretation: 

- "Daily vaccinations" : new doses administered per day (7-day smoothed).
- "Daily vaccinations/million": the number of new doses of vaccinations per million people in the total population of the state received each day.
-  "Total vaccinations": total number of doses administered. This is counted as a single dose, and may not equal the total number of people vaccinated, depending on the specific dose regime (e.g. people receive multiple doses). 

\* Variable interpretation is based on the original interpretation of the raw dataset.
For more detailed information, please refer to: https://github.com/owid/covid-19-data/edit/master/public/data/vaccinations/README.md 

# Python Project 2 
# [Bigfoot Sightings Analysis Report](https://github.com/hattie913/Project-2-Bigfoot/blob/main/Bigfoot_sightings_analysis_report.ipynb)
### Introduction
This report analyzes the Bigfoot records in the United States using Python. We study the Bigfoot sightings across the counties, Bigfoot sightings between 1921 and 2018, narrative of Bigfoot sightings, the comparison between Bigfoot sightings per county and population, and the comparison between Bigfoot sightings per county and mid temperature.

### The Data Set
The original dataset on the Bigfoot sightings in the United States consists of 4747 entries with geographical, climate, date, classification, and observation variables. Other datasets include bigfoot_geo, county data and county labels. A variable check conducted later in the analysis will eliminate data entries that are missing values.

For the details and Python code, please check out [here: python Code](https://github.com/hattie913/Project-2-Bigfoot)
