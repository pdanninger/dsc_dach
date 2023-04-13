# dsc_dach
This repository contains the material for the tutorial at the DSC DACH conference.


# Setup
Clone this repo on a local machine or a server. Next use the dsc_env.yaml file to create the python venv via: `conda env create -f dsc_env.yaml` Afterwards activate the virtual env via: `conda activate dsc_conda`

# Viewing the MLFlow results
To view the results of the trained models use `mlflow ui --backend-store-uri sqlite:///mlruns.db --port 5000 &` and go to http://127.0.0.1:5000/
To stop the running server use `CTRL+C` and type: `pkill -f unicorn` 