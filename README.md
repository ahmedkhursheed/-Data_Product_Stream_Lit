36120 Advanced Machine Learning Application - Spring 2023
==============================

# AT3 Group-7: Data Product with Machine Learning
This project aims to provide users in the USA with a tool to estimate their local travel airfare, allowing them to plan their trips confidently. This README provides an overview of the project, including its objectives, components, and setup instructions.

## Project Overview

### 1. The Brief

You have been tasked to build a data product that will help users in the USA to estimate their local travel airfare better. Users can provide trip details, and the app will predict the expected flight fare.

### 2. Project Components

This project involves building a Streamlit app that allows users to provide the following inputs:

1. Origin airport
2. Destination airport
3. Departure date
4. Departure time
5. Cabin type (coach, premium, etc.)

The key features of this data product include:

- Collecting user input for trip details.
- Predicting flight fares using multiple machine learning models.
- Providing an interface for users to validate their inputs and receive fare estimates.

### 3. Team Collaboration

To ensure the success of this project, the team will need to work together to train four different models. Each student in the group will be responsible for training and submitting their best model.

## Getting Started

To set up the project, follow these steps:

### 1. GitHub Repositories

Each group should set up two private GitHub repositories:

1. **Experimentation Repository (Cookiecutter Data Science Template)**
   - https://github.com/ssandeed/adv_mla_at3_group7_exp
   - This repository will be used to experiment and develop machine learning models following the Cookiecutter Data Science template structure

2. **Streamlit Application Repository**
   - https://github.com/ssandeed/adv_mla_at3_group7_streamlit
   - This repository will be dedicated to the Streamlit application development.

### 2. Model Training

Model training is a crucial part of our project, where each student in the team is responsible for training one of the four machine learning models. Below are the details of each model:

- **Single-Layer Neural Network**: This model was trained using a single-layer neural network architecture. It aims to provide accurate airfare estimates based on the user's input parameters.

- **Random Forest**: The Random Forest model uses an ensemble of decision trees to make predictions. It offers robust performance and has shown a Mean Absolute Error (MAE) score of 47.18.

- **Multi-Layer Neural Network**: This model utilizes a multi-layer neural network architecture to predict airfare. It has achieved a MAE score of 56.09.

- **XGBoost**: XGBoost is an ensemble machine learning algorithm that provides high-quality predictions. It achieved a MAE score of 76.89.


### 4. Model Evaluations

The MAE (Mean Absolute Error) score has been used to evaluate the models' prediction accuracy. Lower MAE values indicate better model performance. The evaluation results are as follows:

| Model Name                  | MAE Score |
| --------------------------- | --------- |
| Single Layer Neural Network | 58.49     |
| Random Forest               | 47.18     |
| Multi-Layer Neural Network  | 56.09     |
| XGBoost                     | 76.89     |

## Future Prospects

To make the Airfare Estimation Data Product accessible to a wider audience, we are considering deploying the Streamlit application using Heroku in future. Heroku is a cloud platform that allows for easy deployment and hosting of web applications. By utilizing Heroku, we can make the application available to users on the web without complex infrastructure setup.

### 1. Benefits of Using Heroku

1. **Scalability**: Heroku provides scalable infrastructure, allowing the application to handle varying levels of user traffic.

2. **Continuous Deployment**: Heroku supports continuous deployment, making updating the application with new features and improvements easier.

3. **Add-Ons**: Heroku offers a variety of add-ons for databases, monitoring, and other services, simplifying application maintenance.

4. **Custom Domain Support**: You can use a custom domain name with your Heroku application for a more branded user experience.

### 2. Deploying to Heroku

When the time comes to deploy the Airfare Estimation Data Product to Heroku, we will provide detailed instructions on setting up the application on the platform. This will include any necessary configuration and deployment steps.

## Usage

Once the project is set up, users can follow these steps to utilize the Airfare Estimation Data Product:

1. Input the origin airport, destination airport, departure date, departure time, and cabin type.
2. Validate the inputs.
3. The Streamlit application will call the trained machine learning models and return the estimated flight fares.

## Conclusion

The evaluation of our machine learning models revealed valuable insights into their performance. The Random Forest model displayed robust predictive capabilities with a notably low Mean Absolute Error (MAE) score of 47.18, making it a strong candidate for accurate airfare estimation. The Multi-Layer Neural Network, although exhibiting an MAE score of 56.09, demonstrated the potential of deep learning techniques in improving prediction accuracy. While XGBoost exhibited a higher MAE score of 76.89, it contributed diversity to our model ensemble. Overall, our models present a range of strengths, paving the way for providing users with reliable airfare estimates for their travel plans.

## Support and Issues

If you encounter any issues or have questions about this project, please use the project-specific GitHub repositories to communicate with the team members.


Project Organization
------------

    ├── LICENSE
    ├── Makefile           <- Makefile with commands like `make data` or `make train.`
    ├── README.md          <- The top-level README for developers using this project.
    ├── data
    │   ├── external       <- Data from third-party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling.
    │   └── raw            <- The original, immutable data dump.
    │
    ├── docs               <- A default Sphinx project; see sphinx-doc.org for details
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks          <- Jupyter notebooks. Naming convention is a number (for ordering),
    │                         the creator's initials, and a short `-` delimited description, e.g.
    │                         `1.0-jqp-initial-data-exploration`.
    │
    ├── references         <- Data dictionaries, manuals, and all other explanatory materials.
    │
    ├── reports            <- Generated analysis as HTML, PDF, LaTeX, etc.
    │   └── figures        <- Generated graphics and figures to be used in reporting
    │
    ├── requirements.txt   <- The requirements file for reproducing the analysis environment, e.g.
    │                         generated with `pip freeze > requirements.txt`
    │
    ├── setup.py           <- makes project pip installable (pip install -e .) so src can be imported
    ├── src                <- Source code for use in this project.
    │   ├── __init__.py    <- Makes src a Python module
    │   │
    │   ├── data           <- Scripts to download or generate data
    │   │   └── make_dataset.py
    │   │
    │   ├── features       <- Scripts to turn raw data into features for modelling
    │   │   └── build_features.py
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── predict_model.py
    │   │   └── train_model.py
    │   │
    │   └── visualization  <- Scripts to create exploratory and results-oriented visualizations
    │       └── visualize.py
    │
    └── tox.ini            <- tox file with settings for running tox; see tox.readthedocs.io


--------

<p><small>Project based on the <a target="_blank" href="https://drivendata.github.io/cookiecutter-data-science/">cookiecutter data science project template</a>. #cookiecutterdatascience</small></p>
