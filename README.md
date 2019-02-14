Using this as the basis of the node application:
https://nodejs.org/en/docs/guides/nodejs-docker-webapp/


Upon every commit in this git repo, dockerhub will automatically pull and build the docker-image.
https://cloud.docker.com/repository/docker/mikemcmillan/test


On Windows:

choco install minikube

minikube start

minikube create deployment docker-helloworld --image=mikemcmillan/test:latest

kubectl port-forward deployment/docker-helloworld 8080:8080

start http://localhost:8080

##kubectl apply ./kube/


For a GUI:
kubectl dashboard
