# generatedata-docker-kube
Deploying generatedocker via docker-compose, and Kubernetes

## To deploy on Docker (2 linked containers)

`$ cd docker`

`$ docker-compose up -d`

generatedata should then be accessible at http://localhost:8000

## To deploy on Kubernetes

`$ cd kubernetes`

Make any changes to the files in this directory that are relevant to your specific environment & requirements (e.g. passwords, naming conventions, etc.). Also consider security/access considerations e.g. whether this capability should sit inside its own Kubernetes namespace

A simple deployment would be just

`$ kubectl apply -f mysql-deployment.yaml,generatedata-deployment.yaml,generatedata-service.yaml`
