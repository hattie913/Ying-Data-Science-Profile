# Ying's Data Science Profile

## Project Demo

---

# Deep Learning Project 1
## [Malaria Detection Using AI-based Tool](https://github.com/hattie913/Malaria_Detection_CNN_Model/blob/main/Notebook_Malaria_Detection_Full_Code.ipynb)

### Introduction 
Traditional manual microscopic diagnosis of malaria is time-consuming and can produce variable results depending on the observer. This project introduces an AI-based malaria detection model leveraging Convolutional Neural Networks (CNNs) to accurately identify malaria parasites (achieving 98.4% accuracy) in blood smear microscopic images.

**Key Questions**:
1. Can a CNN-based ML model detect parasites in red blood cells?
2. How accurately can the CNN model classify malaria-infected and uninfected red blood cells?
3. How can an AI-based solution streamline malaria detection?
4. How can this solution assist in monitoring malaria prevalence?

The detected blood cell images are preprocessed by HSV transformation with Gaussian blurring, which reduces image noise and enhances the model's ability to differentiate parasites from cell impurities under varying microscopic lighting conditions. The final CNN model was enhanced with LeakyReLU and Batch Normalization.

### Data Description
The dataset contains:
- **Training Set**: 24,958 images
- **Test Set**: 2,600 images

Categories:
- **Parasitized**: Contains Plasmodium parasites (12,582 images in training, 1,300 in test set)
- **Uninfected**: No parasites (12,376 images in training, 1,300 in test set)

**Acknowledgements**: Dataset sourced from [National Institutes of Health (NIH)](https://www.nih.gov/), containing 27,558 cell images (accessed on 11 August 2022).

---

# Deep Learning Project 2
## Street View Housing Number Digit Recognition(https://github.com/hattie913/DeepLearning_SVHN-digit-recognition/blob/main/SVHN_Digit_Recognition_GitVersion.ipynb)

### Project Overview
This project aims to develop a neural network model to recognize digit images from the **SVHN (Street View House Numbers)** dataset. This dataset contains over 600,000 labeled digits cropped from street-level photos, making it an excellent resource for training models to automate address transcription, thereby enhancing map applications by identifying building addresses from street images.

### Objective
The goal is to accurately predict the digit in each image. We explore various architectures, including **Artificial Neural Networks (ANN)** and **Convolutional Neural Networks (CNN)**, and select the best-performing model.

### Dataset
We use a subset of the SVHN dataset in `.h5` format for computation efficiency, consisting of:
- **Training Data**: 42,000 images
- **Testing Data**: 18,000 images
- **Validation Data**: 60,000 images

### Methodology
**Data Preprocessing**:
- **Resizing and Normalization**: Each `32x32` pixel image is flattened to a 1D vector of 1024 elements and normalized between 0 and 1.
- **One-Hot Encoding**: Labels are converted to one-hot encoded vectors for multi-class classification (0-9 digits).

**Model Architectures**:
1. **ANN**: A basic ANN with two hidden layers was built, yielding 67% validation accuracy but struggling with complex patterns.
2. **CNN**:
   - **First Model**: Two convolutional layers and Max Pooling layer. Showed overfitting, achieving 87% validation accuracy.
   - **Second Model**: Added convolutional layers, Batch Normalization, and Dropout, resulting in better generalization and high accuracy across training and validation sets.

**Training and Evaluation**:
The models were trained using **backpropagation and the Adam optimizer**. Accuracy and loss were tracked to monitor convergence and detect overfitting.

### Results and Observations
- The **second CNN model** achieved 91% test accuracy, closely matching validation accuracy.
- Precision, Recall, and F1-Scores confirmed robustness, particularly in classes like `0` and `7`.
- **CNN models outperformed the ANN**, demonstrating the advantage of CNNs for image recognition tasks requiring spatial awareness.

### Conclusion
This project demonstrates the power of **Convolutional Neural Networks** for real-world visual data. The second CNN model was optimal for digit recognition in the SVHN dataset, validating CNNs as specialized architectures for complex visual tasks.

---

# Data Analysis and Data Visualization Project 1
## [Restaurant Marketing Analysis](https://github.com/hattie913/Restuarant-Marketing-Analysis/blob/main/FDS_Project_github.ipynb)

### Introduction
A food aggregator company has stored data on various orders made by registered customers on their online portal. This project analyzes customer demand for different restaurants and cuisines, providing data-driven insights to foster growth and improve customer experiences.

### Data Description 
The dataset, in `.csv` format, contains various attributes related to food orders.

---

# Data Analysis and Data Visualization Project 2
## [Bigfoot Sightings Analysis Report](https://github.com/hattie913/Project-2-Bigfoot/blob/main/Bigfoot_sightings_analysis_report.ipynb)

### Introduction
This report examines Bigfoot sightings in the United States using Python, covering sighting patterns across counties from 1921 to 2018, narrative analysis, population comparisons, and mid-temperature correlations.

### Data Description
The original dataset includes 4,747 entries, containing geographic, climate, date, classification, and observation variables. Other related datasets include **bigfoot_geo**, **county data**, and **county labels**. Missing values were addressed during preprocessing.

For full details, see the [Python Code](https://github.com/hattie913/Project-2-Bigfoot).

---

# Python Dashboard Project
## [Covid19 Python Dashboard](https://ma705covid19-project.herokuapp.com/)

The dashboard "Realtime Covid-19 Cases and Vaccinations in Most Populous States in the United States" is deployed on Heroku: [Visit Dashboard](https://ma705covid19-project.herokuapp.com/)

**Python Code**: [GitHub Link](https://github.com/hattie913/ma705-Project-PythonDashboard)

### Dashboard Description
The dashboard tracks daily Covid-19 cases and vaccinations in populous US states since January 2021. Users can observe and compare changes in vaccination implementation and daily Covid-19 counts over time through an interactive time-series graph, with detailed information available in a table below.

### Data Sources
Data was sourced from:
- [Centers for Disease Control and Prevention](https://covid.cdc.gov/covid-data-tracker/#cases_casesper100klast7days)
- [Our World in Data](https://ourworldindata.org/us-states-vaccinations)

- **Covid-19 Cases Dataset**: [CDC API](https://data.cdc.gov/resource/9mfq-cb36.json)
- **Vaccination Dataset**: [US Vaccinations](https://github.com/owid/covid-19-data/tree/master/public/data/vaccinations)

The `realtime_Covid.py` script processes and merges data from these sources, cleaning and transforming it for analysis. The final dataset is saved as a `.pkl` file for downstream analysis.

### Variable Interpretation
- **"Daily vaccinations"**: New doses administered per day (7-day smoothed).
- **"Daily vaccinations/million"**: New doses per million people in the state population.
- **"Total vaccinations"**: Cumulative doses administered.

For more information, visit [Our World in Data Documentation](https://github.com/owid/covid-19-data/edit/master/public/data/vaccinations/README.md).
