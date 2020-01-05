# ml-docker-devops

Learning to expose machine learning service as an API and to build a production grade docker application using flask and flassger.
<br><br>
Dataset - IRIS
<br><br>
# Steps to use
Make sure docker is already installed in your systems.If not click [here](https://docs.docker.com/install/linux/docker-ce/ubuntu/)!!

```
git clone https://github.com/icapucap/ml-docker-devops.git
cd ml-docker-devops/
cd Docker-deployment/
cd Docker\ deployment/
```
Now we build the docker image from the Dockerfile. This may take a while :P
```
sudo docker build -t rf-api .
```
 Now we create a docker container from the docker image we just created
 ```
 sudo docker run -d -p 8000:8000 rf-api
 ```
 Use this command to check whether your container is up and running
 ```
 sudo docker ps
 ```
Now open up your browser and type  localhost:8000/apidocs 
 

