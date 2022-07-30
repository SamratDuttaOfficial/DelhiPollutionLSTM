
# Predicting Delhi's Polution With LSTM

Collaborators: 
[Samrat Dutta](https://github.com/SamratDuttaOfficial),
[Sagar Biswas](https://github.com/mr-sagar-biswas), 
[Tithi Makar](https://github.com/Tithimakar)

Air pollution is responsible for many health problems in the urban areas.
Of late, the air
pollution status in Delhi has undergone many changes in terms of the levels of pollutants and the control measures taken to reduce them.
In this model We have used the artificial recurrent neural network (RNN) architecture Long Short-Term Memory (LSTM) to predict the polution level of delhi in the upcoming days.

## Abstract

The aim of this project is to predict the air pollution trend for future days using a set of past data. Nowadays as a result of globalization pollution is a global threat. 
Air pollution refers to the release of pollutants into the air—pollutants that are detrimental to human health and the planet as a whole.
According to the World Health Organization (WHO), each year air pollution is responsible for nearly seven million deaths around the globe.
Nine out of ten human beings currently breathe air that exceeds the WHO’s guideline limits for pollutants, with those living in low- and middle-income countries suffering the most.

## Authors

- [Samrat Dutta](https://github.com/SamratDuttaOfficial)
- [Sagar Biswas](https://github.com/mr-sagar-biswas)
- [Tithi Makar](https://github.com/Tithimakar)

## Technology

**RNN:** As explained in this article, an RNN takes many input vectors to process them and output other vectors.
It can be roughly pictured like in the image below, imagining each rectangle has a vectorial depth and other special hidden quirks in the image below.
In our case, the "many to one" architecture is used: we accept time series of feature vectors (one vector per time step) to convert them to a probability vector at the output for classification.
Note that a "one to one" architecture would be a standard feedforward neural network.

**LSTM:** Long Short Term Memory is a kind of recurrent neural network.
In RNN output from the last step is fed as input in the current step. 
LSTM was designed by Hochreiter & Schmidhuber. It tackled the problem of long-term dependencies of RNN in which the RNN cannot predict the word stored in the long-term memory but can give more accurate predictions from the recent information. 
As the gap length increases RNN does not give an efficient performance.
LSTM can by default retain the information for a long period of time. 
It is used for processing, predicting, and classifying on the basis of time-series data.


## Time Series Properties
- Window Size: 365 Days.
- Features: 365 Days of the Time-series Data.
- Label: 366th Day's Data.

## Original dataset
We have collected the data from Central Control Room for Air Quality Management - All India.
(https://app.cpcbccr.com/ccr/#/caaqm-dashboard-all/caaqm-landing).

In our experiment, we only used the data from CRRI Mathura Road, Delhi – IMD, from 01/01/2018 to 31/03/2021 for PM 2.5 and PM 10. 

## Process
We executed the experiment in the below process:
1. Data cleaning.
2. Data visualization.
3. Data smoothening.
4. Data processing.
5. Building The Machine Learning model.
6. Training the Machine Learning model.
7. Data Forecasting.

In this process we have used Python programming Language.


## Requirements and Installation
- [Tensorflow](https://www.tensorflow.org/install/)
- [NumPy](https://numpy.org/doc/stable/user/install.html)
- [matplotlib](https://matplotlib.org/)
- [sklearn](https://scikit-learn.org/stable/)
- [Pandas](https://pandas.pydata.org/)

## Data Visualization

**Raw Data**

![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/raw_data.png)

**After Smoothening**
![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/after_smoothening.png)

## Real Value vs  Our Predicted Value

**PM2.5**

![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/real_vs_pred_pm_2.5.png)

**PM10**
![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/real_vs_pred_pm_10.png)

## Forecasting future using The Model

**PM2.5**

![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/future_forecast_pm_2.5.png)

**PM10**

![App Screenshot](https://raw.githubusercontent.com/SamratDuttaOfficial/DelhiPollutionLSTM/master/future_forecast_pm_10.png)

## 🚀 GitHub
Please visit the Github repository to download and see this project.

https://github.com/SamratDuttaOfficial/DelhiPollutionLSTM

Pull requests are always welcome.



