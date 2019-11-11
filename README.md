# Google_Kubernetes_Engine_Project
Application and development using Google Kubernetes Engine. Intermediate process and implementation. Architecture definition and load balancing.

---
## Introduction to Google Kubernetes Engine
To understand what Kubernetes and Kubernetes Engine work for:

1) Bare Metal: They are the physical servers. In addition to managing our application, we must take care of the infrastructure (everything related to Hardware: networks, memory, CPU, etc.) and the operating system (updates, security patches, etc).

2) Virtual Machine: The infrastructure is controlled by a virtualized layer, we do not care more about the physical part of our servers.

3) Containers: Containers are the most optimal operation of our applications. We only care about managing our application and its dependencies (programming languages, frameworks, logs, etc.), while our cloud providers will be in charge of the infrastructure and the operating system.

---

## What is Kubernetes?
Kubernetes Engine is Google’s managed solution on the Google Cloud Platform. Its function is to manage the cluster of machines, the installation of the clients and all the processes for the deployment of our applications. Google takes care of everything.

This tool has the following functionalities:

* Docker Format: Our machines and containers must use this format to be deployed.

* Auto-scaling: The performance of our application will not be affected when many users enter at the same time. You can support all this burden without generating your virtual machines by hand.

* Stackdriver: The Google monitoring and control solution. It helps us to understand very easily what is happening in the infrastructure: logs, alerts, CPU and memory monitoring, etc.

* Cloud VPN: It allows us to have a hybrid cloud with which we will have our data and applications segregated in the cloud and using information from our local servers. All these processes safely.

* Cloud IAM: User administration thanks to Google authentication support. We can assign permissions and roles of reading, writing and administration on our cluster.

### Advantages of Kubernetes Engine:
* Automatic Updates
* Auto repair
* Private container registration
* Uniform and fast versions
* GPU support

### Alternatives:
* Redhat Openshift
* Docker swarm
* Amazon Elastic Container Service for Kubernetes
* IBM Cloud Kubernetes Service
* Azure Kubernetes Service (AKS)

---
## What are the containers?
The name of containers comes from standardized cargo containers that are used in ships, trucks and trains, which allow loading, unloading and stacking containers over long distances, facilitating the transfer from one means of transport to another.

These containers have been a real revolution in the world of transport, reducing costs, loading / unloading times, damage to goods, etc.

Docker takes this same concept to the world of software, allowing to encapsulate any architecture, making it a portable and self-sufficient container, so that it can be manipulated through established operations and run consistently on any hardware.

---
## What is Docker?
Docker is an open source technology, developed in the GO programming language, using the Apache 2.0 license (we can deploy our application on any server, without our source code being open source).

Docker uses the features of UNIX operating systems to manage containers and the deployment of our applications in the memory area of the Linux operating system.

---
## Basic Docker Commands
### Spring framework Petclinic
#### Example instructions
*   ```
    ./mvnw jetty:run-war
    ```
*   ```
    docker run -p 8080:8080 springcommunity/spring-framework-petclinic
    ```

### Docker Commands
* Download and save the images of our application:
    ```
    docker pull
    ```
* List the images downloads on our machine: 
    ```
    docker images
    ```
* List the containers running on our machine (id, port, etc):
    ```
    docker ps
    ```
* List the containers turned off of our machine:
    ```
    docker ps -a
    ```
* Enter our container and list the folders within it:
    ```
    docker exec
    ```
* Stop the execution of our container:
    ```
    docker stop
    ```
* Clear our container:
    ```
    docker rm
    ```