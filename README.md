# Build a Docker Image and Push to DockerHub using Ansible

In this demo, we will be installing docker and building a docker image for an Flask application. Also, the image built will be pushed to DockerHub using ansible playbook. In short, this playbook easily allows you to build and push a docker image to DockerHub.

## Architecture


## Overview

In this demo, we will be provisioning the following :

- Install packages: git, docker and its required dependencies to run the playbook.
- Clone the git repository to remote build server.
- Login to the dockerHub, build and push the image to DockerHub.

## Features

- Easily allows you to build a docker image for an application and push this same image to dockerHub.
- The image build will only take place if there is any change in the contents present in Git repository.

## Requirements

- Install Ansible on your machine (ansible master).
- DockerHub account.

## Variables Used

```
git_url: "https://github.com/Freeda-F/docker-flask-app.git" #--------Git repo URL-------#
docker_username: "freedafrancis"  #--------DockerHub username-------#
docker_password: "**********" #--------DockerHub password-------#
image: "devops-flaskapp"  #--------Image name-------#
version: "v1"
```

## Provisioning



## Usage

## Result






