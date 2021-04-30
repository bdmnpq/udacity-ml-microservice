[![CircleCI](https://circleci.com/gh/bdmnpq/udacity-ml-microservice.svg?style=svg)](https://circleci.com/pipelines/gh/bdmnpq/udacity-ml-microservice)

## Project Overview

In this project, you will apply the skills you have acquired in this course to operationalize a Machine Learning Microservice API. 

You are given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project tests your ability to operationalize a Python flask app—in a provided file, `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

### Project Tasks

Your project goal is to operationalize this working, machine learning microservice using [kubernetes](https://kubernetes.io/), which is an open-source system for automating the management of containerized applications. In this project you will:
* Test your project code using linting
* Complete a Dockerfile to containerize this application
* Deploy your containerized application using Docker and make a prediction
* Improve the log statements in the source code for this application
* Configure Kubernetes and create a Kubernetes cluster
* Deploy a container using Kubernetes and make a prediction
* Upload a complete Github repo with CircleCI to indicate that your code has been tested

You can find a detailed [project rubric, here](https://review.udacity.com/#!/rubrics/2576/view).

---

## Setup the Environment
* Run git clone 'https://github.com/bdmnpq/udacity-ml-microservice.git`
* Run `python3 -m venv ~/.devops`
* Run `source ~/.devops/bin/activate`
* Run `make install` to install the necessary dependencies

### Install Docker
* Create docker account
* Install docker
* Run 'docker --version'

### Install Kubernetes
* Install VirtualBox
* Install minikube

### Configure Kubernetes to Run Locally
* run `minikube start`

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

### Kubernetes Steps

* Setup and Configure Docker locally
* Setup and Configure Kubernetes locally
* Create Flask app in Container
* Run via kubectl

## File list
* Dockerfile: a text document that contains all the commands a user could call on the command line to assemble an image
* Makefile: a text document that defines set of tasks to be executed
* app.py: a python script to predict housing prices
* make_prediction.sh: a bash file to make prediction
* requirement.txt: a text document that contains all the required packages
* run_docker.sh: a bash script to run app.py in Docker
* run_kubernetes.sh: a bash script to run app.py in Kubernetes
* upload_docker.sh: a bash script to upload docker image into docker repo
* model_data: a directory that contains input for prediction
* output_txt_files: log output from both docker and Kubernetes run

