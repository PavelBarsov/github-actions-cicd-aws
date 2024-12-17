# **GitHub Actions deploy Flask-app to AWS Elastic Beanstalk**

---

**Status of Last Deployment:**  
<br> <img src="https://github.com/USERNAME/REPOSITORY/actions/workflows/ci-cd-pipeline.yml/badge.svg?branch=main"><br>

---

## **Overview**

This repository implements a **CI/CD pipeline** using GitHub Actions to automate the deployment of a Flask application to **AWS Elastic Beanstalk**.

The pipeline performs two key stages:

1. **Continuous Integration (CI):**  
   - Builds the application into a ZIP package.  
   - Uploads the package to an S3 bucket.  

2. **Continuous Deployment (CD):**  
   - Creates a new application version in Elastic Beanstalk.  
   - Deploys the version to the target environment.  

---

## **Pipeline Stages**

### **1. Continuous Integration (CI)**  
- Package the Flask app into a deployable ZIP file.  
- Upload the ZIP file to the configured **S3 bucket**.

### **2. Continuous Deployment (CD)**  
- Verify the package in S3.  
- Create a new Elastic Beanstalk application version.  
- Deploy the new version to the target environment.

---

## **Pre-requisites**

To run this pipeline, ensure the following:

1. **AWS Elastic Beanstalk Application**  
   - Configure an Elastic Beanstalk environment and platform.  

2. **S3 Bucket**  
   - Create an S3 bucket for storing application packages.

3. **GitHub Secrets**  
   - Add the following secrets to GitHub:
     - `AWS_ROLE_GITHUB`: IAM role ARN for secure deployment.

4. **OpenID Connect (OIDC)**  
   - Enable OIDC for GitHub Actions in your AWS account.

---
