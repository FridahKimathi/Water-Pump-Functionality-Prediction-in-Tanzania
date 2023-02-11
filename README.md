# Water-Pump-Functionality-Prediction-in-Tanzania

<img src="Images\TanzaniaWater.jpg" alt="A Picture of a tap" width="650" height="400">

##### **Author**: [Fridah Kimathi](mailto:fridahnkirotekimathi@gmail.com)

## Overview
****
The project aims to develop a model to classify the functionality status of water pumps in Tanzania using data sourced by <a href="https://taarifa.org/">Taarifa </a> and the <a href="https://www.maji.go.tz/">Tanzanian Ministry of Water</a>. 

## Business Problem
***
Tanzania is a developing country which is in the midst of a water crisis. The country struggles to provide clean water to its population of over 57 million people despite the fact that the country has many established water points. The Tanzanian government through the Ministry of Water aims at resolving the water crisis in the country by maintaining and repairing the water pumps in time. In order for its Engineers to achieve the objectives faster, they need to be know in advance which water pumps are likely to fail and understand the causes of failure.

The project therefore, aims at developing a model using data collected by <a href="https://taarifa.org/">Taarifa </a> and the <a href="https://www.maji.go.tz/">Tanzanian Ministry of Water</a> to predicts the functionality status of the water pumps in Tanzania as well as provide important insights on the main factors contributing to water pump failure in Tanzania. The model created will enable the Tanzanian Ministry of Water to improve the maintenance operations its water pumps.

## Data
***
The data used in this project is from the <a href="https://www.drivendata.org/competitions/7/pump-it-up-data-mining-the-water-table/page/23/">  Pump it Up: Data Mining the Water Table</a> competition hosted by DrivenData, originally sourced by <a href="https://taarifa.org/">Taarifa </a> and the <a href="https://www.maji.go.tz/">Tanzanian Ministry of Water</a>.


## Modelling
***
Different models were evaluated and the best performing model was picked to be the final model.The Random Forest Classifier was picked as the final model, with its parameters being the best parameters found through grid search. 

                Models
 <img src="Images\models.jpg"  width="650" height="400"> 


## Evaluation
***
The accuracy score of the model is 0.7937. That means that the model predicts the correct water pump functionality status 79.37% of the time.
The most important features according to the final model are age, population, latitude, longitude, gps_height, amount_tsh, permit, public_meeting, district code and region code.

                Accuracy score
 <img src="Images\submission_results.jpg"  width="650" height="400"> 

               Feature importance
<img src="Images\feature_importance.jpg"  width="650" height="400">

              Confusion Matrix
 <img src="Images\cnf_matrix.jpg"  width="650" height="400"> 

## Conclusion
***
The model performed best at the Functional water pumps, did adequately on nonfunctional water pumps, and had the most trouble correctly predicting the functional but needs repair water pumps.The model needs more data especially on nonfunctional/need repair water pumps for it to make an even better prediction. The features identified as the most important can be presented to the stakeholders(The government of Tanzania), to help them improve the maintenance/repair operations of water pumps.

## Limitations
***
The overall data used was not up to date and was not reliably gathered, it contained a lot of placeholders in important features such as population and amount_tsh, hence the results obtained are not particularly accurate. 

## Recommendations
***
<ul> <li>Work with the local government to ensure more accurate gathering of data</li>
<li>Data collected should highlight more on non_functional pumps or those in need of repairs</li>
<li>Data collected could highlight functional pumps that are unlikely to fail</li>
</ul>


## For More Information

See the full analysis in the [Jupyter Notebook](https://github.com/FridahKimathi/Water-Pump-Functionality-Prediction-in-Tanzania/blob/main/index.ipynb) or review this [presentation](https://github.com/FridahKimathi/Water-Pump-Functionality-Prediction-in-Tanzania/blob/main/Water%20Pump%20Functionality%20Prediction%20-Presentation%20PPT.pdf).

For additional info, contact Fridah Kimathi at [fridahnkirotekimathi@gmail.com](mailto:fridahnkirotekimathi@gmail.com) or via my [LinkedIn profile](https://www.linkedin.com/in/fridah-kimathi-91608418b/).



## Repository Structure

```
├── Data
├── Images
├── README.md
├── Water Pump Functionality Prediction 
└── index.ipynb
```
