# SampleApp CI/CD Pipeline with Jenkins and Docker

## Overview
This project demonstrates a simple Jenkins pipeline to build, test, deploy a Node.js application using Docker.

## Jenkins Pipeline
- **Build:** Installs dependencies using `npm install`.
- **Test:** Runs tests with a placeholder command.
- **Docker Build & Push:** Builds Docker image and pushes to Docker Hub.
- **Deploy:** Stops any existing container and runs the new image on port 3000.

## How to Trigger Pipeline
Push any changes to the main branch of this repo. Jenkins is configured to trigger the pipeline on code commit.

## Deployment
The app is deployed in a Docker container running on the Jenkins node at port 3000.

## How to Access
Open a browser and navigate to `http://<jenkins-node-ip>:3000` to see the app in action.

---

### Step 3: Commit and push your changes

- Add the deployment stage to your Jenkinsfile.
- Create and add README.md.
- Commit everything and push to GitHub.

---

Ask if you want me to generate the exact updated Jenkinsfile or README.md content files for you! Ready to proceed with these?
