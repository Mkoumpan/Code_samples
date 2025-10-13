# Prediction of daily Covid-19 hospitalizations and deaths using CNN-LSTMs. Datathon submission


**Introduction**

ABOUT THE DATATHON

The COVID-19 Houston Datathon is an online challenge to predict the regional hospitalization and mortality patterns of COVID-19 in Houston, Texas. This Datathon is jointly 
organized and sponsored by the Center for Secure Artificial intelligence For hEalthcare at the UTHealth School of Biomedical Informatics, and Data to Knowledge lab at 
Rice University. Undergraduate, master, and doctoral students from the institutes within the Gulf Coast Consortia (including UTHealth, MDACC, UH, Rice, TAMU, UTMB, IBT, 
and Baylor) and colleges near TMC are highly encouraged to apply. The event will have up to $1,500 in prizes for the winners. This is an individual-based event (no team 
participation).



**Objective**

The goal is to develop a prediction model using local county-level data to estimate the changes in hospitalization and mortality rates in the greater Houston area encompassing
8 counties (Harris, Fort Bend, Montgomery, Brazoria, Galveston, Liberty, Chambers, and Austin) in the state of Texas, USA.


For further information please read the Notebook "Datathon.ipynb".

**STAR**

Situation: There was a need for Covid-19 hospitalization and death forecasting for 1-2 weeks ahead of time for hospitals. We were given hospitalizations and deaths data directly from hospitals for 8 Counties in Texas.

Task: The task was to forecast the time-series data for a 2-week time period.

Action: I used a recurrent deep neural network such as an LSTM and ConvLSTM to train the model with a varying window of 3-5 days. The model was able to capture long-term dependencies (e.g. 1 week) as well as short-term dependencies such as less cases in the weekend.

Solution: I evaluated my model using various metrics such as rmse, mae, mse.


**Execution**

The program can be executed as follows:

-- Upload on Google Colab or run using Jupyter Notebooks

**References**
1. https://sbmi.uth.edu/datathon/past-events/aug20.htm

**Languages Used**

Python 3.7

**License**

All the code belongs to the University of Houston. Copying and redistribution is not allowed.

