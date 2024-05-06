# Starting a FastAPI Project with HELM

This repository contains the HELM configuration files to deploy an application created in python with FastAPI, this is what you have to do to execute the commands and view the application 

## Pasos

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

##### En MacOs y Linux:

```Powershell
source venv/bin/activate
```

#### 1.3 Instalar FastAPI y Uvicorn:

Con el entorno virtual activo, instala FastAPI y Uvicorn, que es el servidor ASGI recomendado para ejecutar aplicaciones FastAPI.

```Powershell
pip install fastapi uvicorn
```

#### 1.4 crear un archivo "requirements.txt"

Si ya sabes qué bibliotecas adicionales necesitas, puedes crear un archivo requirements.txt manualmente y listarlas allí. Por ejemplo:

```
fastapi==0.68.0
uvicorn==0.15.0
```
