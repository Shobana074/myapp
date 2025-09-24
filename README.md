# SampleApp CI/CD Pipeline with Jenkins and Docker

## Overview
This project demonstrates a simple Continuous Integration and Continuous Deployment (CI/CD) pipeline using Jenkins and Docker.

The pipeline automates:
- Building the Node.js application.
- Running basic tests.
- Building a Docker image and pushing it to Docker Hub.
- Deploying the app automatically as a Docker container.

## Jenkins Pipeline Stages

1. **Build:** Installs dependencies using `npm install`.
2. **Test:** Runs tests (currently a placeholder).
3. **Docker Build & Push:** Builds the Docker image and pushes to Docker Hub repository `shobs074/sampleapp`.
4. **Deploy:** Stops any running container named `sampleapp` and runs the new Docker image on port 3000.

## How to Trigger the Pipeline
The pipeline is triggered automatically on every code commit pushed to the `main` branch of this GitHub repository.

## Deployment Details
- The app is deployed on the Jenkins build node inside a Docker container.
- The container exposes port 3000 to access the running app.

## Accessing the App
Open a browser and navigate to:
http://<jenkins-node-ip>:3000

Replace `<jenkins-node-ip>` with the IP address or hostname of your Jenkins server.

## Tools Used
- Jenkins for automation.
- Docker for containerization.
- Node.js application as the sample app.

## How to Use This Project
1. Clone this repository.
2. Push any code changes to trigger the pipeline.
3. Use the Jenkins dashboard to monitor builds.
4. Access the running application via Docker container on port 3000.

