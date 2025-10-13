# Prediction of daily Covid-19 hospitalizations and deaths using CNN-LSTMs. Datathon submission


## Introduction

ABOUT THE DATATHON

The COVID-19 Houston Datathon is an online challenge to predict the regional hospitalization and mortality patterns of COVID-19 in Houston, Texas. This Datathon is jointly 
organized and sponsored by the Center for Secure Artificial intelligence For hEalthcare at the UTHealth School of Biomedical Informatics, and Data to Knowledge lab at 
Rice University. Undergraduate, master, and doctoral students from the institutes within the Gulf Coast Consortia (including UTHealth, MDACC, UH, Rice, TAMU, UTMB, IBT, 
and Baylor) and colleges near TMC are highly encouraged to apply. The event will have up to $1,500 in prizes for the winners. This is an individual-based event (no team 
participation).



# COVID-19 Hospitalization and Mortality Forecasting

## Overview
This project focused on forecasting COVID-19 hospitalizations and deaths 1–2 weeks ahead of time to support hospitals in resource allocation and preparedness. The data consisted of hospitalization and mortality records collected from hospitals across eight counties in Texas.

---

## Situation
There was an urgent need for accurate short-term forecasts of COVID-19 hospitalizations and deaths to help hospitals manage capacity and allocate medical resources effectively. Hospitals across eight Texas counties provided real-time data on daily hospitalizations and deaths, which formed the basis for this modeling effort.

---

## Task
The objective was to develop a time-series forecasting model capable of predicting hospitalizations and deaths up to two weeks into the future. The challenge involved capturing both short-term trends (e.g., weekday-weekend fluctuations) and longer-term patterns in the evolving pandemic data.

---

## Action
- **Model Development:** Implemented deep recurrent architectures including **LSTM** and **ConvLSTM** networks using TensorFlow to model temporal dependencies in the data.  
- **Feature Engineering:** Used a variable time window (3–5 days) to capture different temporal patterns and smooth out noise in the daily reports.  
- **Training and Tuning:** Performed hyperparameter optimization to balance model complexity and generalization.  
- **Evaluation:** Compared performance across models and time windows using cross-validation and held-out data.

---

## Result
The models successfully captured both long-term dependencies (e.g., weekly trends) and short-term variations such as reduced weekend case counts.  
Evaluation using **RMSE**, **MAE**, and **MSE** demonstrated consistent and robust performance across the eight counties, providing reliable forecasts that could inform hospital operations and planning.

---

## Technologies Used
- **Python**, **TensorFlow**, **NumPy**, **Pandas**
- **Matplotlib / Seaborn** for visualization
- **LSTM** and **ConvLSTM** architectures for time-series modeling



**Execution**

The program can be executed as follows:

-- Upload on Google Colab or run using Jupyter Notebooks

**References**
1. https://sbmi.uth.edu/datathon/past-events/aug20.htm

**Languages Used**

Python 3.7

**License**

All the code belongs to the University of Houston. Copying and redistribution is not allowed.

