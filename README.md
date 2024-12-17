# GitHub Actions deploy Flask-app to AWS Elastic Beanstalk

Status of Last Deployment:<br>
<img src="https://github.com/PavelBarsov/github-actions-cicd-aws/actions/workflows/main.yml/badge.svg?branch=main"><br>

Overview
This repository implements a CI/CD pipeline using GitHub Actions to automate the deployment of a Flask application to AWS Elastic Beanstalk.

The pipeline performs two key stages:

Continuous Integration (CI): Builds and uploads the application to S3.
Continuous Deployment (CD): Creates a new application version and deploys it to Elastic Beanstalk.
