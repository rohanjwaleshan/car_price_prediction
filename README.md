# Car Selling Price Predictor: Project Overview
* Created a regression model that predicts a car's selling price (average r-squared = 0.91, average rmse = 234541 rupees) so individuals interested in selling their car have an easier time deciding a selling price for their car.
* The dataset used to train the model was from [Kaggle](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho?select=Car+details+v3.csv). The dataset consists of information about used cars from CarDekho (a website where users can sell or purchase cars in India).
* 7906 cars in dataset (before cleaning)
* Performed necessary cleaning steps on data such as, removing missing values and removing unrealistic values (selling_price, mileage, etc.)
* Formatted categorical features into useable features (Units for mileage, engine, and max_power were removed and then converted to numerical data. The name of each car was converted to the country it orginated from.) for multiple linear regression model and decision tree model
* Exploratory data analysis consisted of checking for strong linear association between features and the response through correlation heatmap and scatterplots.
* Model assumptions for multiple linear regression were checked and cross validation was performed for the decision tree model to assess generalization.

## Code
**Python Version**: 3.8.8<br />
**Packages**: numpy, pandas, matplotlib, seaborn, sklearn, statsmodels, scipy<br />
**Requirements**: `pip install -r requirements.txt`

## Data
Dataset from [Kaggle](https://www.kaggle.com/nehalbirla/vehicle-dataset-from-cardekho?select=Car+details+v3.csv) consists of information about used cars from CarDekho (a website where users can sell or purchase cars in India).
* **name** - name of the car
* **year** - year the car was purchased
* **selling_price** - the car's selling price
* **km_driven** - number kilometers the car has driven
* **fuel** - fuel type (Diesel, Petrol, CNG, LPG)
* **seller_type** - whether the car was sold by an individual or dealer                 ![first 5 rows of dataset](dataset.png)
* **transmission** - the car's gear transmission (Automatic/Manual)
* **owner** - number of previous owners
* **mileage** - mileage of the car
* **engine** - car's engine capacity
* **max_power** - max power of engine (bhp)
* **torque** - car's torque
* **seats** - number of seats in the car

