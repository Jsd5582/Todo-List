
# Project Week 7: Deploying to-do list front-end microservice on a cloud cluster

## Introduction
As of now, you have completed Project Week 6 and should now have an understanding of the regular development of a fully functional to-do-list Application. For Project Week 7, you will go through the process of understanding containerizing the microservice and the process of deploying the to-do-list front-end microservice component on an IBM cloud cluster.


## Containerizing microservice
- Developing in microservices is the art of breaking down the old model of building one large application, i.e., a "monolithic" application, and forming a new model where specialized, cloud-hosted sub applications—each charged with a very specific task—work together. For this, we have added a `frontendserver.js` using express.
- Containers are a standard way to package an application and all its dependencies so that it can be moved between environments and run without change. Docker is one of the most popular Containerization platforms, which allows you to develop, deploy, and run the application inside containers. We have created a Dockerfile to containerize the to-do-list front-end application. **Note**: Below commands are just for your understanding.
- We have then built the docker image and tagged it using the below command.
```
docker build -f Dockerfile -t ibmaccelerate/cloudnative:frontend_v1 .
```
- The Image is pushed to the docker hub. You will be using this already built image to deploy on your cluster.




## Instructions
