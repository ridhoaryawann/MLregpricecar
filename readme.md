![Header](header.png)

## About

Executive Summary

This machine learning project aims to predict used car prices in support of the Saudi Green Initiative (SGI), which promotes the transition from gasoline cars to electric vehicles (EVs). The high cost of EVs is a significant barrier to adoption, so the government plans to subsidize the transition by buying used cars at market value plus a 50% premium. Accurate price predictions are crucial for fair and competitive buyback processes, fostering trust and participation in the program. 

We solve this problem by developing a regression model that accounts for various factors affecting car prices, such as condition, age, brand, and mileage. Our primary metric for evaluation is Mean Squared Error (MSE), ensuring that the model's predictions are inclusive and fair for the majority of the population. By minimizing MSE, we aim to align predicted prices with market rates, thereby supporting the program's success and the broader goal of reducing transportation emissions. 

**Context**

The Saudi Green Initiative (SGI) is a national effort led by His Royal Highness Prince Mohammed bin Salman bin Abdulaziz, Crown Prince and Prime Minister, to combat climate change and enhance the environment. Launched in 2021, SGI aims to achieve net zero emissions by 2060 through a Circular Carbon Economy approach, while also promoting a green economy. SGI focuses on reducing emissions, increasing afforestation, and protecting land and sea areas.

**Trade Your Car to Electric Vehicle Program**

Aligned with the Saudi Green Initiative's emissions reduction objective, a key strategy is encouraging individuals to swap their conventional gasoline cars for electric vehicles (EVs). This initiative dovetails with the broader goal of transitioning towards a sustainable, low-carbon future. 

Under this program, the government purchases used cars from citizens at market price plus a 50% premium, using the proceeds to acquire EVs for participants. This incentivizes the shift to EVs, significantly reducing transportation emissions while promoting clean energy and automotive innovation. 

**Problem Statement**

A significant hurdle to EV adoption is their high pricing. To mitigate this, the government plans to subsidize by buying used cars and exchanging them for EVs, offering a 50% premium above market value. However, determining accurate market prices is challenging due to various factors, such as vehicle condition, age, brand, and etc. 

The government aims for fair and competitives pricing strategy to ensure program success and equitable buyback processes, enabling effective and fair operation for all community. 

**Goals**

Given these challenges, the Saudi government requires a tool to predict and assist individuals in determining appropriate prices for their used cars. Variances in features like engine type, manufacturing year, brand, vehicle type, and mileage can enhance buyback price accuracy, ensuring program success.

Accurate price predictions are crucial for program success. When predicted prices closely align with market rates, participation in the buyback or trade-in program for EVs hopefully will increases. Moreover, fair price predictions build trust in the government's execution of the program, also fostering increased participation.

**Analytic Approach**

Therefore, our task is to analyze data to identify patterns among the existing features that differentiate one used car from another.

Subsequently, this pattern will be used to develop a regression model to assist the user (Saudi Arabian government) in providing a prediction tool for purchasing prices of used cars, which will be instrumental in implementing the buyback program.

**Metric Evaluation**

We prioritize MSE to ensure the model accommodates most of car used by Saudi Arabia population, aiming for inclusive predictions. While RMSE, R2, and MAPE indicator will also be important, we want to maintain MSE score as minimal as possible to make sure the predictive part is fair for most of the Saudi people.

RMSE that emphasize on outlier will not be as effective as MSE in predicting most of Saudi people car that had not have a change to afford the sport cars or the classic car. 

**Model Selection and Implementation**

Given the context of the data, with many outliers and high cardinality, robust and tree-based models are suitable choices. Here are the steps to create and implement the model:

Data Preprocessing: Handling missing values, encoding categorical variables, and scaling numerical features.
Model Selection: Using robust models such as Ridge Regression, Lasso Regression, Random Forest, and XGBoost to handle outliers and high cardinality.
Training and Evaluation: Splitting the data into training and testing sets, training the models, and evaluating them using the chosen metrics.
Hyperparameter Tuning: Using techniques such as GridSearchCV to optimize model performance.
Deployment: Creating a uinterface for government officials to input car details and receive price predictions.

## Installation

To get this project, you can clone it by running the following code:

    git clone git@github.com:ridhoaryawann/MLregpricecar.git

    
## Project Organization

The directory structure of Machine Learning Regression project looks like this:

    ├── README.md          <- README for developers using this project.
    │
    ├── docs               <- The document will consist of:
    │   └── data_saudi_used_cars.csv : raw data.
    │
    ├── src                <- Source code for use in this project.
    │   └── 1)business_eda.ipynb: business & eda understanding 2)model_experiment.ipynb: model creation, interpretation and │        recommendation
    │
    ├── pickle             <- Directory to store the serialized machine learning models.
    │   └── used_car_price_predictor.pkl : Serialized model file. 

## Contribute

If you'd like to contribute to IndoMarket Apps, check out https://github.com/ridhoaryawann/MLregpricecar.git, or feel free to contact me.