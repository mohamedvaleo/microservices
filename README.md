https://circleci.com/gh/mohamedvaleo/microservices.svg?style=svg

## Project Summary

Operationalize this working, machine learning microservice using kubernetes, which is an open-source system for automating the management of containerized applications.

## Installation

* Create a virtualenv and activate it
   python3 -m venv ~/.devops
   source ~/.devops/bin/activate
* Run `make install` to install the necessary dependencies

### Other Libraries

* Docker
* Hadolint 
* Kurbernetes (Minikube)

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`

## Project Files

* docker_out.txt: include the log output after a prediction is made, given some sample input data
* kubernetes_out.txt: include the log output after a prediction is made, given some sample input data
* run_kubernetes.sh: create local cluster configured and running
* run_docker.sh: Run a Container & Make a Prediction
* requirements.txt: include all the dependencies needed to run the application app.py
* app.py: the actual application code which make the prediction.
* Makefile: includes instructions on environment setup and lint tests
* Dockerfile: container code which include the base image and all the dependencies
* config.yml: the pipeline code which will be executed by the circleCI
