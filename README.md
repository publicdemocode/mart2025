# mart2025

How to run simple demo application

from demo2703/k8s folder

connect to k8s cluster and run one by one following commands
be sure command run successfully before running the next one - I mean to verify the kubernetes resource is created and running

kubectl apply -f 1-pod-postgres.yaml  
kubectl apply -f 2-svc-postgres.yaml  
kubectl apply -f 3-pod-valkey.yaml  
kubectl apply -f 4-svc-valkey.yaml  
kubectl apply -f 5-cm.yaml  
kubectl apply -f 6-job.yaml  
kubectl apply -f 7-app.yaml  
kubectl apply -f 8-pod-scheduler.yaml  
kubectl apply -f 9-pod-scheduler.yaml  
kubectl apply -f 10-svc-app.yaml  

the last command should create Load Balancer its ip you can check by
kubectl get svc
note the external ip and try to connect in browser
