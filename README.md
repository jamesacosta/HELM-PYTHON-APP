# Starting a FastAPI Project with HELM

This repository contains the HELM configuration files to deploy an application created in python with FastAPI, this is what you have to do to execute the commands and view the application 
#### REMEMBER IT IS POSSIBLE NOT TO SEE THE APPLICATION BECAUSE IT WORKS WITH A MONGODB ATLAS CLUSTER.
## STEPS

### 1. Clone this repository using 

```bash
git clone https://github.com/jamesacosta/HELM-PYTHON-APP.git
```
 
#### 1.1 We move to the folder that contains the most important files for this run

```bash
cd /fasapi-helm/templates
```

#### 1.2 we enter this page and perform the correct installation of HELM  

```Powershell
https://helm.sh/docs/intro/install/
```

#### 1.3 we enter this page and perform the correct installation of MINIKUBE, which is a local kubernetes cluster.

```Powershell
https://minikube.sigs.k8s.io/docs/start/
```

#### 1.4 execute the commands to create a namespace and execute the other command to start running the application

```Powershell
# Create a namespace if necessary
kubectl create namespace [NAMESPACE_NAME]
# Deploy the chart
helm install [DISPLAY_NAME] [CHART_ROUTE] --namespace [NAMESPACE_NAME]
# You can use this command
helm install [DEPLOY_NAMESPACE] [CHART_ROUTE] --namespace [NAMESPACE_NAME] -f values.yaml
```

#### 1.4 To terminate the process use this command  
```Powershell
# Delete Deploy
helm uninstall [DEPLOY_NAME] --namespace [NAMESPACE_NAME]
```
