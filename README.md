# Optimizing-Agricultural-Productio

### Problem Statement 
To predict the best cultivable crop for Suitable land and whether

##### Description for each of the columns in the Dataset

- N - ratio of Nitrogen content in soil
- P - ratio of Phosphorous content in soil
- K - ration of Potassium content in soil
- temperature - temperature in degree Celsius
- humidity - relative humidity in %
- ph - ph value of the soil
- rainfall - rainfall in mm


## Descriptive Statistics

- Average Ratio of Nitrogen in the Soil : 50.55
- Average Ratio of Phosphorous in the Soil : 53.36
- Average Ratio of Potassium in the Soil : 48.15
- Average Tempature in Celsius : 25.62
- Average Relative Humidity in % : 71.48
- Average PH Value of the soil : 6.47
- Average Rainfall in mm : 103.46

## Analyzing Agricultural Conditions

![image](https://user-images.githubusercontent.com/82017895/122646930-55596980-d13f-11eb-9cf6-ebe41c52b2f2.png)

Some Interesting Patterns
---------------------------------
- Crops which requires very High Ratio of Nitrogen Content in Soil: ['cotton']
- Crops which requires very High Ratio of Phosphorous Content in Soil: ['grapes' 'apple']
- Crops which requires very High Ratio of Potassium Content in Soil: ['grapes' 'apple']
- Crops which requires very High Rainfall: ['rice' 'papaya' 'coconut']
- Crops which requires very Low Temperature : ['grapes']
- Crops which requires very High Temperature : ['grapes' 'papaya']
- Crops which requires very Low Humidity: ['chickpea' 'kidneybeans']
- Crops which requires very Low pH: ['mothbeans']
- Crops which requires very High pH: ['mothbeans']
-----------------------------------
* Summer Crops
['pigeonpeas' 'mothbeans' 'blackgram' 'mango' 'grapes' 'orange' 'papaya']
-----------------------------------
* Winter Crops
['maize' 'pigeonpeas' 'lentil' 'pomegranate' 'grapes' 'orange']
-----------------------------------
* Rainy Crops
['rice' 'papaya' 'coconut']
-----------------------------------

## Clustering Similar Crops

![image](https://user-images.githubusercontent.com/82017895/122647040-ec262600-d13f-11eb-867e-f9323c9793e3.png)

Lets check the Results After Applying the K Means Clustering Analysis 

Crops in First Cluster: ['maize' 'banana' 'watermelon' 'muskmelon' 'papaya' 'cotton' 'coffee']
---------------------------------------------------------------
Crops in Second Cluster: ['grapes' 'apple']
---------------------------------------------------------------
Crops in Third Cluster: ['maize' 'chickpea' 'kidneybeans' 'pigeonpeas' 'mothbeans' 'mungbean'
 'blackgram' 'lentil' 'pomegranate' 'mango' 'orange' 'papaya' 'coconut']
---------------------------------------------------------------
Crops in Forth Cluster: ['rice' 'pigeonpeas' 'papaya' 'coconut' 'jute' 'coffee']
---------------------------------------------------------------

Results for Hard Clustering

Crops in Cluster 1: ['cotton', 'watermelon', 'banana', 'muskmelon', 'maize']
--------------------------------------------------
Crops in Cluster 2: ['grapes', 'apple']
--------------------------------------------------
Crops in Cluster 3: ['pomegranate', 'kidneybeans', 'chickpea', 'mango', 'orange', 'lentil', 'blackgram', 'mungbean', 'mothbeans']
--------------------------------------------------
Crops in Cluster 4: ['coconut', 'papaya', 'jute', 'pigeonpeas', 'rice', 'coffee']
--------------------------------------------------


## visualizing the Hidden Patterns

![image](https://user-images.githubusercontent.com/82017895/122647116-3c04ed00-d140-11eb-96c0-21a6a2d8087f.png)

## Predictive Modelling

![image](https://user-images.githubusercontent.com/82017895/122647161-6a82c800-d140-11eb-8f5d-b9e3aaec34ba.png)


## Real time Predictions

- For prediction = model.predict((np.array([[90,
                                       40,
                                       40,
                                       20,
                                       80,
                                       7,
                                       200]])))
- The Suggested Crop for Given Climatic Condition is : ['rice']
