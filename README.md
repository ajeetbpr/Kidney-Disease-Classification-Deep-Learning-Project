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


## AWS-CICD-Deployment-with-Github-Actions

### 1. Login to AWS console

### 2. Create IAM user for deployment

```
#with specific access

1. EC2 access : It is virtual machine

2. ECR: Elastic Container registry to save your docker image in aws


#Description: About the deployment

1. Build docker image of the source code

2. Push your docker image to ECR

3. Launch Your EC2 

4. Pull Your image from ECR in EC2

5. Lauch your docker image in EC2

#Policy:

1. AmazonEC2ContainerRegistryFullAccess

2. AmazonEC2FullAccess
```
### 3. Create ECR repo to store/save docker image
```- Save the URI: 566373416292.dkr.ecr.us-east-1.amazonaws.com/chicken```

### 4. Create EC2 machine (Ubuntu)

### 5. Open EC2 and Install docker in EC2 Machine:
```
#optinal

sudo apt-get update -y

sudo apt-get upgrade

#required

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker
```
### 6. Configure EC2 as self-hosted runner:
```- setting>actions>runner>new self hosted runner> choose os> then run command one by one```

### 7. Setup github secrets
```
AWS_ACCESS_KEY_ID=

AWS_SECRET_ACCESS_KEY=

AWS_REGION = us-east-1

AWS_ECR_LOGIN_URI = demo>>  566373416292.dkr.ecr.ap-south-1.amazonaws.com

ECR_REPOSITORY_NAME = simple-app