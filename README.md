# DevOps Project

Here is our final devops-project.

## 1. Work performed

### 1. Unit tests

We used Mocha and Chai dependencies. We performed 15 tests including 7 User tests and 5 User REST/API tests.

### 2. CI/CD pipeline using Travis CI & Heroku 

We choosed to apply CI/CD pipeline using [Travis CI](https://travis-ci.com/github/RaphaelBhnk/devops-project)  for the CI part, and [Heroku](https://devops-project1.herokuapp.com) platform for the CD part.

### 3. Provision a virtual environment and run our application using iaC approach

We created a virtual machine with one distribution of Linux : centos. We created several tasks: 
-Health check of our application.
-Installation of our database: Redis.
-Installation of Node.js.

We synced our application on the host machine tio the guest machine.

### 4. Docker image of our application

We created the Docker image of our application : devops-project available [here]https://hub.docker.com/repository/docker/weepizz/devops-project_web) on Docker Hub.

### 5. Container orchestration using Docker Compose

We added our docker-compose.yaml file which start our containers and so the application.

### 6. Docker orchestration using Kubernetes

We created the k8s folders, which contains all our .yaml Kubernetes files needed for the containers orchestration.

## 2. Instructions 

### Installation, Usage & Testing : 

Start application:
```
# Clone the repository

git clone https://github.com/RaphaelBhnk/devops-project

# Download the dependencies

cd devops-project
npm install

# Start the development server
npm start
```

Run tests:
```
npm test
```

Vagrant:
```
cd iaC
vagrant up
```
Docker-compose:
```
docker-compose up
```
Kubernetes: 
```
cd k8s
minikube start
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f pv-claim.yml
kubectl apply -f pv-volume.yaml
```
## 3. Necesseray links with the platforms and tools integrated: 

| Realisations | URL |
|---------|-------|
| Travis CI :  | https://travis-ci.com/github/RaphaelBhnk/devops-project |
| Heroku deployment : | https://devops-project1.herokuapp.com |
| Docker Hub : | https://hub.docker.com/repository/docker/weepizz/devops-project_web |

## 4. Authors

Raphael BOUHNIK 
raphael.bouhnik@edu.ece.fr

Adrien ZYCHOWSKI 
adrien.zychowski@edu.ece.fr