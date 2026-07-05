# Sample App CI/CD Pipeline – Final Project

This repository contains my implementation of the Final Project for the Coursera course **CI/CD Tools and Practices**. It demonstrates a complete CI/CD pipeline for a sample Flask microservice, including:

- **Continuous Integration** with GitHub Actions (linting with flake8, unit testing with nosetests)
- **Continuous Deployment** with Tekton pipelines and OpenShift, including build, lint, test, and deploy tasks
- Deployment verification on an OpenShift cluster with application logs and pipeline run screenshots

## Usage
This repository is to be used as a template to create your own repository in your own GitHub account. No need to Fork it as it has been set up as a Template. This will avoid confusion when making Pull Requests in the future.
From the GitHub **Code** page, press the green **Use this template** button to create your own repository from this template.
Name your repo: `ci-cd-final-project`.

## Setup
After entering the lab environment you will need to run the `setup.sh` script in the `./bin` folder to install the prerequisite software.
```bash
bash bin/setup.sh
```
Then you must exit the shell and start a new one for the Python virtual environment to be activated.
```bash
exit
```

## Tasks
- Implemented GitHub Actions workflow (`.github/workflows/workflow.yml`) with lint (flake8) and unit test (nosetests) jobs.
- Implemented Tekton tasks (`.tekton/tasks.yml`) including cleanup, clone, lint, and test tasks.
- Configured and ran an OpenShift Pipeline (`oc-pipeline`) to build, test, and deploy the application.
- Verified successful pipeline runs and application deployment on OpenShift with PVC, pipeline logs, and application logs.

## License
Licensed under the Apache License. See [LICENSE](/LICENSE)

## Author
Loviiii

## <h3 align="center"> © IBM Corporation 2023. All rights reserved. <h3/>
