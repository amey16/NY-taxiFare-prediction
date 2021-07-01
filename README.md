# NY-taxiFare-prediction
Predicting the taxi fare and the fare class using regression and classification

# Dataset
- This is a kaggle dataset and a very interesting one indeed - [kaggle link](https://www.kaggle.com/c/new-york-city-taxi-fare-prediction/data) 
- This particular project revolves around only 120000 rows of train.csv .If you need the simplified dataset clone the repo and use taxi-fare.csv 
- Command to clone the repository
```
git clone "https://github.com/amey16/NY-taxiFare-prediction.git"
```
- fare_amount feature would be the target for regression models rest would be training features
- fare_class would be the target class for classification models

# Repo Structure
- part1 has preprocessing and regression,ANN implementation with hyper-parameter tuning
- part2 has Implementation of TPOT regressor a very cool tool
- part3 consists of classification might surprise you with the accuracy

# Stuff I learnt
- Haversine distance
    - Distance between two points with given latitude and longitudes 
    - Takes in consideration the sperical surfaces
    - [How it works](https://www.geeksforgeeks.org/haversine-formula-to-find-distance-between-two-points-on-a-sphere/)
- TPOT automated library
    - A very useful thing that automatically decides which regressor/classifier is the best
    - Just be careful t choose affordable params else you might have to wait 2 days 
    - [To read about it](http://epistasislab.github.io/tpot/using/)

- Storing the dataset in mongodb
    - the finaldata was saved in mongodb for later use
    - data was converted into json key value pairs and the pairs were added using insertmany 
    - To do so first you have to download the mongodb compas [website](https://www.mongodb.com/try/download/community)
    - click on the on premises/server option then download according to your laptop configuration 
    - For rest follow the steps done in part1.ipynb
    
- Just a extra comment (Never work in this large datasets with pc configurations like mine) :wink:
