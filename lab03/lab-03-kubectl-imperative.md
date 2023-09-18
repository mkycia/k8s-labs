# LAB-03

```
1. kubectl run test123 --image=busybox -- sleep 3600

2. kubectl get pods 
   kubectl get pods --selector run=test123

3. kubectl create deployment nginx123 --image=nginx --replicas=3

4. kubectl get pods
   kubectl get pods --selector app=nginx123

5. kubectl describe pod test123

6. kubectl describe deployment nginx123
```