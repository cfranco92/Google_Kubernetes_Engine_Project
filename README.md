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