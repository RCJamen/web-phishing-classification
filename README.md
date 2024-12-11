# Phishing Website Classification using Machine Learning

## Overview
This project focuses on the classification of phishing websites using machine learning techniques. Phishing attacks remain a major cybersecurity threat, often tricking users into providing sensitive information by mimicking legitimate websites. Machine learning models are employed to detect phishing sites based on various URL attributes, aiming to enhance real-time protection and detection accuracy in combating such threats.

## Problem Statement
Phishing websites are increasingly difficult to differentiate from legitimate sites, making it essential to develop reliable methods for their detection. Traditional security systems may fail to identify phishing attempts effectively. This project utilizes machine learning classifiers to automatically assess the legitimacy of websites and identify potential phishing threats based on URL-based features.

## Dataset
The dataset used for training the model contains features extracted from both phishing and legitimate websites. It consists of 111 attributes—96 derived from the website URL itself and 15 custom features extracted via Python scripts. The dataset includes 88,647 instances, with 30,647 labeled as phishing and 58,000 as legitimate websites. Data sources include PhishTank (for phishing sites) and Alexa's top websites (for legitimate sites). The features are categorized into URL properties, domain properties, directory properties, file properties, and parameter properties.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/RCJamen/web-phishing-classification
    cd web-phishing-classification
    ```

2. Create and activate virtual environment:
    ```bash
    python -m venv .venv
    source .venv/bin/activate  # For Linux/Mac
    # or
    .venv\Scripts\activate  # For Windows
    ```

3. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1. Run the Jupyter notebook:
    ```bash
    jupyter notebook analytics.ipynb
    ```

## Model Architecture
This project employs several machine learning classifiers, including Random Forest (RF), Gradient Boosting (GB), K-Nearest Neighbors (KNN), and Gaussian Naive Bayes (GNB). These models are trained to classify websites as either phishing or legitimate based on their URL attributes. Hyperparameter tuning is performed using GridSearchCV to optimize model performance.

## Features
The following features are utilized in the classification model:
- **URL Properties**: Various characteristics of the entire URL string.
- **Domain Properties**: Attributes derived from the website's domain name.
- **Directory Properties**: Features representing the structure of the URL directories.
- **File Properties**: Characteristics of the file extensions used in the URL.
- **Parameter Properties**: Analysis of URL parameters for anomalies.



## Model Performance
The model is evaluated using the following metrics:
- **Precision**: The proportion of true positive predictions to all positive predictions.
- **Recall**: The proportion of true positive predictions to all actual positive instances.
- **F1-score**: The harmonic mean of Precision and Recall, providing a balance between the two.

Actual performance metrics may vary depending on the dataset and training conditions. The results for each model are summarized in the performance table.

## Author
Ramel Cary B. Jamen (2019-2093)

## Acknowledgments
The author would like to thank Dr. Orven Llantos for his expertise and guidance throughout the Data Mining and Analysis course. Special thanks to the contributors and dataset providers, including PhishTank and Alexa, for making the data available.

