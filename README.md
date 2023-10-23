# Kidney-Disease-Classification-Deep-Learning-Project
Kidney-Disease-Classification-Deep-Learning-Project-MLflow-DVC

## Workflows
1. Update config.yaml
2. Update secrets.yaml [Optional]
3. Update params.yaml
4. Update the entity
5. Update the configuration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the dvc.yaml
10. app.py


## Start the project:
```
1. conda create -p kidney  python=3.9 -y
```
```
2. conda activate /Users/ajeetsingh/Documents/ML/Kidney-Disease-Classification-Deep-Learning-Project/kidney
```
```
3. pip install -r requirements.txt 
```

## Run the project:

## DagsHub
MLFLOW_TRACKING_URI=https://dagshub.com/ajeetbpr/Kidney-Disease-Classification-Deep-Learning-Project.mlflow \
MLFLOW_TRACKING_USERNAME=ajeetbpr \
MLFLOW_TRACKING_PASSWORD=2ed593b21375fd3e32e3d1129bddbbd26983efa1 \
python script.py

### Export following environment variables from terminal
export MLFLOW_TRACKING_URI=https://dagshub.com/ajeetbpr/Kidney-Disease-Classification-Deep-Learning-Project.mlflow

export MLFLOW_TRACKING_USERNAME=ajeetbpr

export MLFLOW_TRACKING_PASSWORD=2ed593b21375fd3e32e3d1129bddbbd26983efa1


## DVC Commands
1. dvc init
2. dvc repro (it will run pipeline one by one)

