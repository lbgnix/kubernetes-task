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
