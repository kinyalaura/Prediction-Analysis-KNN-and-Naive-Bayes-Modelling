# Prediction-Analysis-KNN-and-Naive-Bayes-Modelling
# Titanic Prediction K-Nearest Neighbour model.
![Titanic_image](https://data.ibtimes.sg/en/full/17883/titanic.jpg?w=800)

## Table of Contents:

* Data Set
* Result

## Data Set
Below are the features provided in the Test dataset.
 
Train.csv will contain the details of a subset of the passengers on board (891 to be exact) and importantly, will reveal whether they survived or not, also known as the “ground truth”.
 
The `test.csv` dataset contains similar information but does not disclose the “ground truth” for each passenger. It’s your job to predict these outcomes.
 
Using the patterns you find in the train.csv data, predict whether the other 418 passengers on board (found in test.csv) survived


### Categorical Features
*  Passenger Id: and id given to each traveler on the boat
* Pclass: the passenger class. It has three possible values: 1,2,3 (first, second and third class)
* The Name of the passenger
* Sex
* The ticket number
* The cabin number
* The embarkation. This describes three possible areas of the Titanic from which the people embark. Three possible values S,C,Q
 
### Numerical Features
* Age
* SibSp: number of siblings and spouses traveling with the passenger
* Parch: number of parents and children traveling with the passenger
* The ticket Fare

### Target Variable
* Survived - binomial observations (0 - not survived,1 - survived)

### Result
model type | Accuracy Score | Recall(0,1)| Precision(0,1) | F1 (0,1) | AUC curve
-----------|----------------|------------|----------------|----------|--------
RandomForest | 0.83| 0.88, 0.77| 0.86, 0.79 | 0.87, 0.78 | 0.82
KNN without Optimization | 0.77 | 0.78, 0.75 | 0.86, 0.63|0.82, 0.69| 0.75
KNN (80% training)| 0.79 | 0.82, 0.75| 0.85, 0.71| 0.84, 0.73| 0.78
KNN (70% training)|0.78 | 0.82, 0.72| 0.84, 0.70| 0.85, 0.71| 0.77
KNN (60% training)|0.78 | 0.80, 0.75| 0.86, 0.65| 0.83, 0.69|0.76
