# DevOps Assigment 2 - GitHub Actions & DockerHub

# Description of Workflow

## Build (steps)
- Set up job (Began the job)
- Run actions/checkout@v3
- Run actions/setup-java@v3
- Execute Gradle build (Begin the build)
- Copy Jar file
- Run actions/upload-artifact@master
- Post Run actions/setup-java@v3
- Run actions/checkout@v3
- Complete job (Build complete)


## Build Image
- Set up job (Began the job)
- Run actions/download-artifact@master
- Set up Docker Buildx
- Login to Docker Hub (Login into docker, this allows for the docker push to happen)
- Build and push (Push updates to the docker repository)
- Post Login to Docker Hub (Push build)
- Post Set up Docker Buildx
- Complete job (Image is built)




## Link to DockerHub Repository
[DockerHub - `aunspaw-WOPro-Service`](https://hub.docker.com/repository/docker/haunspaw3/aunspaw-wopro-service/general)

## Link to GitHub Actions Run Results Summary
[Link to **working** workflow run results](https://github.com/WSU-kduncan/devops-assignment-2-3-haunspaw/actions/runs/11657452483/job/32455065957)
