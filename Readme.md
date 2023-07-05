# This is the MiniKube Environment  Mern app Deployment
### The architecture:
![image](https://github.com/HitanshuGupta/mern-app-with-k8s/assets/72181617/4d3c3381-6acd-4a6a-a6c5-65d8bbca8012)

### The result:
![image](https://github.com/HitanshuGupta/mern-app-with-k8s/assets/72181617/b377bd5d-83c6-4c53-907b-b93aba405fbc)

#### For set-up, the Control Plane (Master) and Worker Node Use these commands.
```
apt-get install kubectl   
apt-get install minikube  
```
++++++++++++++++++++++++++++++++++++++
#### These are some commands which use for creating the pod.
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
#### To start the service
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
### Reference : https://kubernetes.io/docs/home/ 