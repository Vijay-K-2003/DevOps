# Kubernetes Commands

## Create a deployment of a specific image
```
kubectl create deployment nginx-deployment --image=nginx
```
## Show pods
```
kubectl get pods
```
## Show deployments
```
kubectl get deploy
```
## Show namespaces
```
kubectl get namespaces
```
## Show services
```
kubectl get services
```
## Scale a deployment
```
kubectl scale deployment nginx-deployment --replicas=5
```
## Delete a pod
```
kubectl delete pod nginx-pod
```
## Exposing a deployment using NodePort
```
kubect expose deployment nginx-deployment --type=NodePort --port=8080 --target-port=80
```
## Deleting namespaces
```
kubectl delete namespaces <namespacename>
```
## Change namespace
```
kubectl config set-context --current --namespace=<namespacename>
```
## View current config
```
kubectl config view
```
## Delete all pods in a namespace
```
kubectl delete --all pods --namespace=<name>
```
## Delete all deployments in a namespace
```
kubectl delete --all deployments --namespace=<name>
```
## Delete all namespaces
```
kubectl delete --all namespaces
```
 