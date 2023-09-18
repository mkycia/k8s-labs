# LAB-10

```
1. kubectl create deployment mydb --image=mariadb --replicas=1

2. kubectl get pods		        # proszę zwrócić uwagę na status Error i CrashLoopBackOff

3. kubectl describe pod mydb-xxx-xxx

4. kubectl logs mydb-xxx-xxx

5. kubectl set env deploy/mydb MARIADB_ROOT_PASSWORD=secret
```