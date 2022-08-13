# kubernetes-task

# CMD To Practice of kubernetes on Minikube development environment
```
minikube start --no-vtx-check

kubectl create deployment hello-minikube --image=k8s.gcr.io/echoserver:1.4
kubectl expose deployment hello-minikube --type=NodePort --port=8080
kubectl get services hello-minikube
minikube service hello-minikube
minikube service hello-minikube --url
minikube dashboard

kubectl delete service hello-minikube
kubectl delete deployment hello-minikube
```
# To create YAML from Dry Run command 
#To Create Yaml of POD-

```
kubectl run redis --image=redis123 --dry-run -o yaml

kubectl create deployment httpd-frontend --image=httpd:2.4-alpine --replicas=3


kubectl rollout status deploy/httpd-frontend
```
![image](https://user-images.githubusercontent.com/26162869/184503119-359fe073-c273-4605-86c2-dee6c69de3e0.png)

When you wish to deploy an application in Kubernetes, you usually define three components:

A Deployment — which is a recipe for creating copies of your application.
A Service — an internal load balancer that routes the traffic to Pods.
An Ingress — a description of how the traffic should flow from outside the cluster to your Service.
Here's a quick visual recap.

https://learnk8s.io/troubleshooting-deployments
