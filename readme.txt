HIDDEN MARKOV MODEL AND MACHINE LEARNING FOR WEATHER FORECAST


Aim: Predict whether it rains next day based on present day features


Data: From Commonwealth of Australia 2010, Bureau of Meteorology.

This dataset contains about 10 years of daily weather observations from many locations across Australia.



Features(X): 

Temperature, Pressure, Wind Speed, Humidity, Rainfall, etc of present day.


Y: Binary variable(0/1) to predict whether it rains or not next day


Model:  

1. Use K-means clustering algorithm to cluster the training data(features)


2. Use the cluster no as the hidden states of a HMM Model.


3. Calculate emission and transition matrices from (H,E) pairs.

    H: hidden states, E: emissions


    H -> H -> H
    ↓    ↓    ↓
    E    E    E


4. Perform predictions on test set.
