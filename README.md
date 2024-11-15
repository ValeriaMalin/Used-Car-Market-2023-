Germany's Used Car Market Analysis and Price Prediction

This project analyzes and predicts used car prices for the German market. The dataset, scraped from one of the largest car sales platforms in Germany and hosted on Kaggle, includes comprehensive details on used cars sold in 2023. Key attributes of each listing include the car's production year, mileage, power (PS), fuel type, transmission, color, and fuel consumption.

The analysis seeks to uncover patterns, trends, and insights specific to the German used car market, followed by machine learning (ML) models to predict car prices based on various features. This project combines data exploration, visualization, and predictive modeling to gain insights and produce accurate price predictions.

Project Aims

Data Analysis and Visualization:
Understand price distributions: Analyze the price range of used cars to identify average price points and detect any outliers.
Explore attributes: Examine car attributes such as production year, mileage, power, fuel type, transmission, color, and fuel consumption.
Reveal relationships: Discover correlations between the car's price and its characteristics, seeking insights unique to the German market.
Visualize patterns: Create graphs to represent the distribution and relationship of key parameters like mileage, production year, and power with price.
Price Prediction Using Machine Learning:
Develop ML models that leverage the available data to predict car prices based on attributes. The models will be evaluated for accuracy and interpretability.
Dataset

Source: Kaggle - a popular platform for datasets and data science projects.
Contents: The dataset includes key attributes of used cars listed on a major German car sales platform. These attributes allow for in-depth analysis and serve as features for predictive modeling.
Data Collection: The data was scraped from the platform in 2023 and reflects the current trends and characteristics in Germany’s used car market.
Note: Due to potential redistribution limitations, the original dataset is not included in this repository. Users can access the data via Kaggle. Please refer to the Dataset Download Instructions section below.

Features:
Brand: The brand or manufacturer of the car.
Model: The specific model of the car. 
Color: The color of the car's exterior. 
Registration Date: The date when the car was registered (Month/Year). 
Year of Production: The year in which the car was manufactured.
Price in Euro: The price of the car in Euros. 
Power: The power of the car in kilowatts (kW) and horsepower (ps). 
Transmission Type: The type of transmission (e.g., automatic, manual). 
Fuel Type: The type of fuel the car requires. 
Fuel Consumption: Information about the car's fuel consumption in L/100km ang g/km. 
Mileage: The total distance traveled by the car in km. 
Offer Description: Additional description provided in the car offer.


Methodology

Data Cleaning and Preprocessing: Raw data is cleaned and processed to ensure it is ready for analysis and modeling. This includes handling missing values, handling strange values (as 220 l/100 km fuel consumption), converting units where necessary, and feature engineering.
Exploratory Data Analysis (EDA): Visualizations and summary statistics are generated to understand key trends and relationships within the data.
Feature Engineering: Transforming relevant attributes to better capture relationships, including encoding categorical variables and normalizing numerical variables.
Machine Learning Models: Several regression models (e.g., Linear Regression, Random Forest, Decision Tree, k-Nearest Neighbors, XGBoost, CatBoost, LightGBM) are trained to predict car prices. Model performance is evaluated using metrics like r2, Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE). The analysis of errors was perforemd as well.
Insights and Reporting: The findings are summarized, with key insights about the German used car market highlighted.
Results and Insights

Key insights gained from this project include:

Patterns in car prices relative to mileage, production year, and other attributes. Patterns of prices, power levels transmissiona nd fuel types, colors, brand across the years.
Popular attributes in German used cars, such as common brands, models, colors, fuel types, transmission types and typical power levels.
Predictive accuracy achieved through machine learning models and their reliability for estimating car prices based on various attributes.
Getting Started

Project Notebooks

The analysis and modeling in this project are organized into multiple Jupyter notebooks, each covering specific steps in the data exploration, cleaning, and machine learning process. Below is a list of the notebooks and a brief description of what each contains:

1_cars_data_cleaning.ipynb
This notebook handles the data-cleaning process, including removing outliers, handling missing values, and preparing features for analysis and modeling. It also saves the cleaned version of the dataset.
2_cars_exploratory_data_analysis.ipynb
This notebook explores the dataset through visualizations and summary statistics. Key insights include distributions and relationships between features such as mileage, power, production year, and price.
3_cars_data_distribution.ipynb
Studies the distribution of numerical features, examining aspects like outliers, skewness, and kurtosis. This notebook explores the effects of different transformations (log, square root) and scaling techniques (robust scaling) on the distributions to improve symmetry and reduce outlier impact.
4_cars_models_pipeline.ipynb
This notebook conducts a preliminary model screening using a pipeline to evaluate multiple machine learning algorithms (Linear Regression, k-Nearest Neighbors, Decision Tree, Random Forest, XGBoost) with GridSearchCV for hyperparameter tuning. The pipeline also tests various preprocessing modifications on the cleaned data, providing an initial comparison of model performance before more detailed individual model tuning.
5_cars_linear_regression.ipynb
6_cars_knn.ipynb
7_cars_decision_tree.ipynb
8_cars_random_forest.ipynb
9_cars_XGBoost.ipynb
10_cars_catboost_lightgbm.ipynb

The final notebook summarizes the analysis and modeling results. Key findings from the data exploration and model performance are discussed, and visualizations are included to communicate insights about Germany’s used car market.
Prerequisites
Python 3.x and packages like pandas, numpy, matplotlib, seaborn, scikit-learn, and Jupyter Notebook.
Jupyter Notebook (for easy access to code and visualizations).
Dataset Download Instructions
Visit the dataset page on Kaggle: Germany Used Cars Dataset ([provide the exact URL here](https://www.kaggle.com/datasets/wspirat/germany-used-cars-dataset-2023/discussion?sort=hotness
)![image](https://github.com/user-attachments/assets/e3384607-c7d7-47d8-ab60-4e1a1363bb43)
)

Download the dataset and save it to the /data directory within the repository folder (create the folder if it doesn’t exist).
Update the dataset path in the notebook or script as needed to load the data.
Running the Analysis and Model Training
Clone the repository:
git clone https://github.com/ValeriaMalin/Used-Car-Market-2023
cd your-repo-name
Install required packages:
pip install -r requirements.txt
Launch Jupyter Notebook:
jupyter notebook
Open the main analysis notebook (e.g., car_price_analysis.ipynb) to view the analysis and model training process step-by-step.
Repository Structure

my-used-cars-analysis/
│
├── data/                    # Folder for the dataset (not included; see download instructions)
├── notebooks/               # Jupyter notebooks for EDA, visualizations, and ML modeling
├── scripts/                 # Python scripts for data preprocessing and model training
├── report.pdf               # Project report with findings and insights
├── README.md                # Project description, usage instructions, and goals
└── LICENSE                  # License file
License

Code: Licensed under the MIT License, allowing for modification and redistribution with attribution.
Data: Please refer to the Kaggle license and terms of use for dataset redistribution guidelines.
Report: Shared under CC BY 4.0, allowing for sharing and adaptation with attribution.
Contributing

Contributions are welcome! If you’d like to add improvements, feel free to fork the repository and open a pull request.
