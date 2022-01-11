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

##### Install packages: git, docker and its required dependencies to run the playbook.

![image](https://user-images.githubusercontent.com/93197553/148967390-f4f5a7fc-5f10-455d-a11c-ef375e5b3853.png)
![image](https://user-images.githubusercontent.com/93197553/148967542-65902088-055c-46bf-b8c8-e9d6c2d68626.png)


##### Clone the git repository to remote build server.

![image](https://user-images.githubusercontent.com/93197553/148967630-393c7efb-5709-4cc8-847c-61ee1275a965.png)

##### Login to the dockerHub, build and push the image to DockerHub.

![image](https://user-images.githubusercontent.com/93197553/148967751-5e5bd8cb-3c0b-4313-a452-6048ce5f1e9f.png)


## Usage

1. Clone the repository using the below command
```
git clone https://github.com/Freeda-F/docker-build-push-via-ansible.git
```
2. Then, make the required changes for variables mentioned in the above section.

3. Finally, you can run the ansible playbook using the command
```
ansible-playbook -i inventory docker-build-push.yml
```

## Result


![image](https://user-images.githubusercontent.com/93197553/148968145-cb04f6fd-eef8-4bfe-9608-c1925f7925db.png)






