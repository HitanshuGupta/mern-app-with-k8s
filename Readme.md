# This is the MiniKube Environment  Mern app Deployment

### The result : 
![image](https://github.com/HitanshuGupta/mern-app-with-k8s/assets/72181617/b377bd5d-83c6-4c53-907b-b93aba405fbc)

#### For set-up the Control Plane(Master) and Worker Node Use these commaonds.
```
apt-get install kubectl   
apt-get install minikube  
```
++++++++++++++++++++++++++++++++++++++


```
minikube start
kubectl get pod
kubectl apply -f mongo-config.yaml
kubectl apply -f secret.yaml
kubectl apply -f mongo-app.yaml
kubectl apply -f web-app.yaml
kubectl get pod
kubectl get configmap
kubectl get secret
kubectl get svc
minikube ip
kubectl get node -o wide
```

```
minikube service webapp-service
```
++++++++++++++++++++++++++++++++++++++
```
kubectl delete deployment --all
```
```
kubectl delete secret --all
```
