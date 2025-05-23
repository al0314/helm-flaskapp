# 🚀 Helm Chart for Flask Application

This repository contains a Helm chart for deploying a simple Flask application to a Kubernetes cluster.

## 📋 Prerequisites

Before deploying, ensure the following tools are installed and configured:

- [Helm](https://helm.sh/docs/intro/install/) v3 or later
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- Access to a running Kubernetes cluster

## 📦 Getting Started

### Clone the Repository :

~~~bash
git clone https://github.com/al0314/helm-flaskapp.git
cd helm-flaskapp  
~~~

### Install the Helm Chart :
~~~bash  
helm install flaskapp1 .
~~~  
this will deploy the Flask application inside your cluster  

### Upgrade the chart :  
to remove the deployment use
~~~bash
helm uninstall flaskapp1  
~~~

## 🔍 Check Deployment  
Verify the resources created:  
~~~bash
kubectl get all  
~~~ 
## 🌐 Access the Application  
If you want to access the application forward port to your liking   
~~~bash
kubectl port-forward service/flask-service port:5000  
~~~    
## 📚 Resources
- [Helm Docs](https://helm.sh/docs/)

- [Kubernetes Docs](https://kubernetes.io/docs/home/)  

## 🧑‍💻 Author  
Maintained by [al0314](https://github.com/al0314)

