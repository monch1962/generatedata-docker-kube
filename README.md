# generatedata-docker-kube
Deploying generatedocker via docker-compose, and Kubernetes

## To deploy on Docker (2 separate containers)

`$ cd docker`

`$ docker-compose up -d`

generatedata should then be accessible at http://localhost:8000

## To deploy on Kubernetes

`$ cd kubernetes`

`$ kubectl apply -f mysql-deployment.yaml,generatedata-deployment.yaml,generatedata-service.yaml`
