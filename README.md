# Welcome to Andre-Devsecops
This is a guide to help you navigate this repository.

## Github Pipeline status
[![CI processs for andre-devsecops](https://github.com/iilness2/andre-devsecops/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/iilness2/andre-devsecops/actions/workflows/ci.yml)

## Folder Structure
- `.github`: main GitHub Actions directory
- `.github/workflow/ci.yml`: GitHub Actions CI/CD configuration
- `python_application`: Python application, Python dependencies, and Dockerfile directory
- `assets`: Directory for screenshots

## Workflow flow
1.Running application directly from console
- checkout code
- compile dependency and run hello world
Result: ![Run_Hello_World_Directly](assets/Run_Hello_World_Directly.png)
- upload hello world python and dockerfile files as artifact

2. Running application from docker
- login into docker hub
- download artifact for hello world python and dockerfile files from first workflow
- build and push docker image into docker hub
- run image vulnerability scanner for image result using trivy
- running hello world from docker
Result: ![Run_Hello_World_from_Docker](assets/Run_Hello_World_from_Docker.png)

## Docker Image Scanning Step in the Pipeline
Result: ![Run_Hello_World_Directly](assets/Docker_Image_Scanning_Step.png)

## Improvement
- We can upload code scanning results to GitHub. This allows collaborators working on the repository to easily work together to improve the application's security quality
- In addition to Docker image scanning, we can also add Software Composition Analysis (SCA), code quality scanning, Static Application Security Testing (SAST), and Dynamic Application Security Testing (DAST) to improve the overall security and quality of our applications. For more details, you can also check the article I wrote at this [link](https://dev.to/iilness2/perspectives-on-the-evolution-of-devsecops-engineering-based-on-from-my-experiences-21me)

## Contact
Linkedin Link: https://www.linkedin.com/in/iilness/
Website Link: https://campsite.bio/iilness

## Additional Information
Docker Hub URL used for this project: https://hub.docker.com/repository/docker/iilness/andre-devsecops-python/general
