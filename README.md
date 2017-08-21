# About the sample application
The [Microservice Builder](https://developer.ibm.com/microservice-builder/) sample application is a modified fork of the [Microprofile Showcase Application](https://github.com/eclipse/microprofile-conference). Like its parent it's a web application for managing a conference and is based on a number of discrete microservices. The front end is written in Angular; the backing microservices are in Java. All run on WebSphere Liberty, in Docker containers managed by Kubernetes. The sample application demonstrates various Microservice Builder features:
- Microservices running as WebSphere Liberty Docker containers on Kubernetes
- Optional deployment via a Jenkins-based build pipeline
- ELK log stack integration
- Inbound HTTPS out of the box

## Ways to use the sample application

The sample application can be used with or without a [Jenkins](https://jenkins.io/)-based deployment pipeline. It can be run on IBM Cloud private, or on [minikube](https://github.com/kubernetes/minikube). Both of these are distributions of [Kubernetes](https://kubernetes.io/). Developers may wish to start testing the application by deploying its component microservices directly to minikube. Demonstrators might prefer to start with a Jenkins-based approach, deploying either to minikube or IBM Cloud private.

The main installation steps are:

1. Install prerequisite tools
1. Install Kubernetes (minikube or IBM Cloud private)
1. Install the 'fabric' - extra infrastructure services on top of Kubernetes
1. Install the 'sample ELK' - Elasticsearch, Logstash, and Kibana stack for monitoring metrics
1. Optionally install and configure Jenkins
1. Install or deploy the sample application

The exact steps to be taken vary based on which Kubernetes you will be using, and whether or not you intend to use Jenkins. Follow the appropriate link below for further instructions:

* [Direct deployment to minikube without Jenkins](dev_test_local_minikube.md)
* [Running a full pipeline on IBM Cloud private](full_icp.md)
