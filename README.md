[![CircleCI](https://dl.circleci.com/status-badge/img/gh/Johnnasimba/microservice-kubernetes-/tree/master.svg?style=svg)](https://dl.circleci.com/status-badge/redirect/gh/Johnnasimba/microservice-kubernetes-/tree/master)

## MICROSERVICES AT SCALE USING AWS AND KUBERNETES | OPERATIONALIZE MICROSERVICE API

This project involves operationalizing a machine learning microservice API that predicts housing prices in Boston based on several features. The API is developed using `Python Flask` and the project tests the ability to operationalize this app using `Kubernetes`, an open-source system for automating the management of containerized applications. The project involves creating a `Dockerfile` to containerize the application, deploying the container using `Docker` and `Kubernetes`, and improving the log statements in the source code. The end goal is to upload a complete Github repo with `CircleCI` to indicate that the code has been tested. This project can be extended to any pre-trained machine learning model and is not just limited to housing price prediction.

## Running the application
1. Setup a python virtual environment and activate it
  `python3 -m venv ~/.devops`
  `source ~/.devops/bin/activate`
2. Install the necessary dependencies
  `make install`
3. Run the application 
  `python3 app.py`
4. Run in Docker
  `./run_docker.sh`
5. Run in Kubernetes
  `./run_kubernetes.sh`

## Predict housing prices
`./make_predicion.sh`
## Main File

#### app.py
Contains the code for the API(Main application)
#### Dockerfile
Docker container which runs the application 
#### run_docker.sh
Contains code that runs docker container
#### Makefile
Defines the commands to install dependencies and lint the code
#### .circleci/config.yml
CircleCI configuration file 
#### upload_docker.sh
Upload docker image to docker hub
