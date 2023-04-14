# dsc_dach
This repository contains the material for the tutorial at the DSC DACH conference.


# Setup
Clone this repo on a local machine or a server. Next use the dsc_env.yaml file to create the python venv via: `conda env create -f dsc_env.yaml` Afterwards activate the virtual env via: `conda activate dsc_conda`

# Tutorial
The notebook `mlflow_tutorial.ipynb` contains the entire tutorial for several functionalities of MLflow. The tutorial uses the California house price data set to setup a machine learning workflow from data exploration, data preprocessing and training of model with a subsequent versioning of these models using MLFlow. Further, a final model will be registered to the `Production` stage in MLflow and used for prediction of prices of new houses.

# Viewing the MLFlow results
To view the results of the trained models use `mlflow ui --backend-store-uri sqlite:///mlruns.db --port 5000 &` and go to http://127.0.0.1:5000/
To stop the running server use `CTRL+C` and type: `pkill -f unicorn` 