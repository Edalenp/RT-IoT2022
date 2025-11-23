# RT-IoT2022: Intrusion Detection with Classical Machine Learning

This project implements classical machine learning algorithms to detect and classify normal and malicious traffic using the RT-IoT2022 dataset. The goal is to evaluate different ML techniques and analyze their performance in intrusion detection tasks within IoT-based environments.

## Dataset Description

The RT-IoT2022 dataset integrates real IoT devices with modern cyberattack scenarios. It contains:

- **IoT Devices**: ThingSpeak-LED, Wipro-Bulb, MQTT-Temp
- **Attack Types**:
    - SSH brute-force
    - DDoS (Hping, Slowloris)
    - Nmap scanning patterns
- **Features**: Bidirectional network flow attributes extracted with Zeek and Flowmeter

This dataset is designed for studying intrusion detection in resource-constrained IoT systems.

## Project Structure

```
├── data/
│   ├── raw/                 
│   └── processed/           
├── notebooks/               
│   ├── 01_data_understanding.ipynb
│   ├── 02_data_preparation.ipynb
│   ├── 03_modeling.ipynb
│   └── 04_evaluation.ipynb
├── results/
│   ├── figures/             
│   ├── tables/              
│   └── models/               
└── README.md
```
<br>

# Workflow Overview

The project is organized into four main steps, each implemented in a dedicated notebook:

### 1. Data Understanding

- Load and inspect the dataset
- Class distribution analysis
- Descriptive statistics
- Missing value analysis
- Correlation study
- Identification of outliers and noise

### 2. Data Preparation

- Cleaning and preprocessing
- Handling missing values
- Encoding categorical variables
- Feature scaling

### 3. Modeling

- Training classical ML models such as:

    - Logistic Regression
    - Decision Tree
    - Random Forest
    - Support Vector Machine
    - k-Nearest Neighbors
    - Naive Bayes

- Hyperparameter tuning (optional)

### 4. Evaluation

- Confusion matrices
- ROC and AUC
- Accuracy, precision, recall, F1-score
- Comparison of all models
- Final performance summary