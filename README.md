# Ying's-Data-Science-Profile
Project Demo

# Deep Learning Project 1
# [Malaria Detection Using AI-based tool](https://github.com/hattie913/Malaria_Detection_CNN_Model/blob/main/Notebook_Malaria_Detection_Full_Code.ipynb)
### Introduction 
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

# Deep Learning Project: Street View Housing Number Digit Recognition
## Project Overview
This project aims to develop a neural network model capable of recognizing digit images from the **SVHN (Street View House Numbers)** dataset. The SVHN dataset, containing over 600,000 labeled digits cropped from real-world street-level photos, serves as an excellent resource for training models to automate address transcription. This automation can improve map applications by identifying building addresses from street images.
## Objective
The goal is to build a model that can accurately predict the digit within each image. To achieve this, we explore different architectures, including **Artificial Neural Networks (ANN)** and **Convolutional Neural Networks (CNN)**, and select the architecture that yields the best performance.
## Dataset
We use a subset of the SVHN dataset stored in `.h5` format to streamline computations. This subset includes:
- **Training data**: 42,000 labeled images
- **Testing data**: 18,000 images
- **Validation data**: 60,000 images
Each image in the dataset represents a cropped digit from a street view. Before training, the data undergoes several preprocessing steps to prepare the images and labels for effective model training.
## Methodology
### Data Preprocessing
- **Resizing and Normalization**: Each image, originally in a 2D matrix format (`32x32` pixels), is flattened into a 1D vector of 1024 elements to suit the input requirements for the ANN. The pixel values are then normalized to a range between 0 and 1, enhancing the model's training stability.
- **One-Hot Encoding**: Labels are converted into one-hot encoded vectors, allowing the model to perform multi-class classification on ten distinct digit classes (0-9).
- 
### Model Architectures
1. **Artificial Neural Network (ANN)**: 
   - A basic ANN with two hidden layers was constructed to assess performance with a simpler feed-forward architecture. Although it provided a validation accuracy of 67%, it struggled with more complex patterns in visual data.
2. **Convolutional Neural Networks (CNN)**:
   - **First CNN Model**: This initial CNN model, with two convolutional layers and a Max Pooling layer, showed strong training accuracy but exhibited overfitting, resulting in a validation accuracy of 87%.
   - **Second CNN Model**: To address overfitting, a more advanced CNN model was implemented with additional convolutional layers, Max Pooling layers, Batch Normalization, and Dropout layers. This model achieved improved generalization and maintained high accuracy across both training and validation datasets.
   - 
### Training and Evaluation
Each model was trained on the preprocessed dataset using **backpropagation and the Adam optimizer**. The learning rate and batch size were carefully chosen to optimize performance. After training, each model’s accuracy and loss were tracked across epochs to evaluate convergence and potential overfitting.
## Results and Observations
- The **second CNN model** achieved the best results, with a test accuracy of **91%**, aligning closely with its validation accuracy and indicating reliable generalization.
- **Precision, Recall, and F1-Scores** across the test set further confirmed the model’s robustness, with especially high recall for classes such as `0` and `7`.
- The **CNN models significantly outperformed the ANN**, demonstrating that convolutional architectures are far better suited for image recognition tasks where spatial relationships are crucial.
## Conclusion
This project underscores the power of **Convolutional Neural Networks** in handling real-world visual data. The second CNN model, with its high accuracy and ability to generalize, proved optimal for digit recognition in the SVHN dataset. Overall, the CNN models’ performance validated the importance of using specialized architectures for complex visual tasks, with CNNs outperforming ANNs in precision and accuracy.


# Data Analysis and Data Visulization Project 1
# [Restaurant Marketing Analysis](https://github.com/hattie913/Restuarant-Marketing-Analysis/blob/main/FDS_Project_github.ipynb)
### Introduction
The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. This project is to understand the demand of different restaurants/cuisines, and provide data-driven insights for the growth and improvement for a better customer experience.
### Data Description 
The data contains the different data related to a food order and is stored in .csv file.

# Data Analysis and Data Visulization Project 2
# [Bigfoot Sightings Analysis Report](https://github.com/hattie913/Project-2-Bigfoot/blob/main/Bigfoot_sightings_analysis_report.ipynb)
### Introduction
This report analyzes the Bigfoot records in the United States using Python. We study the Bigfoot sightings across the counties, Bigfoot sightings between 1921 and 2018, narrative of Bigfoot sightings, the comparison between Bigfoot sightings per county and population, and the comparison between Bigfoot sightings per county and mid temperature.

### The Data Set
The original dataset on the Bigfoot sightings in the United States consists of 4747 entries with geographical, climate, date, classification, and observation variables. Other datasets include bigfoot_geo, county data and county labels. A variable check conducted later in the analysis will eliminate data entries that are missing values.

For the details and Python code, please check out [here: python Code](https://github.com/hattie913/Project-2-Bigfoot)

# Python Dashboard Project
# [Covid19 Python Dashboard](https://ma705covid19-project.herokuapp.com/)


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
- "Total vaccinations": total number of doses administered. This is counted as a single dose, and may not equal the total number of people vaccinated, depending on the specific dose regime (e.g. people receive multiple doses). 

Variable interpretation is based on the original interpretation of the raw dataset.
For more detailed information, please refer to: https://github.com/owid/covid-19-data/edit/master/public/data/vaccinations/README.md 


