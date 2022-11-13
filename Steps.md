```

docker build -t aditya0709/minikube-react-app:v1 .
[+] Building 3.2s (8/8) FINISHED

docker push aditya0709/minikube-react-app:v1                 
The push refers to repository [docker.io/aditya0709/minikube-react-app]
a449848e04f9: Pushed 
b85443563c06: Pushed 
7c4dfec5a9f2: Pushed 
8d14dc56a724: Pushed 
286ccd57a256: Pushed 
5242cd795028: Pushed 
994393dc58e7: Pushed 
v1: digest: sha256:41ae2bbdeed29e52f47daefe2d3ae53686ca1e537e7a1ad51fa980a0a99b90c9 size: 1778

kubectl apply -f deployment.yaml
deployment.apps/minikube-react-app unchanged
service/minikube-react-app unchanged

kubectl get pods                
NAME                                  READY   STATUS    RESTARTS   AGE
minikube-react-app-5b46b8478f-q5gcq   1/1     Running   0          75s
minikube-react-app-5b46b8478f-qtt8p   1/1     Running   0          75s
```