# LAB-08

```
1. kubectl create cm my1stdbvarscm --from-literal=MYSQL_ROOT_PASSWORD=password 

2. kubectl describe cm my1stdbvarscm

3. kubectl get cm my1stdbvarscm -o yaml

4. kubectl create deploy my1stdb --image=mysql 

5. kubectl set env --from=configmap/my1stdbvarscm deployment/my1stdb

6. kubectl get pods --selector app=my1stdb

7. kubectl create secret generic my1stdbsecrets --from-literal=MYSQL_ROOT_PASSWORD=password 	

8. kubectl describe secret my1stdbsecrets

9. kubectl get secret my1stdbsecrets -o yaml

10. kubectl get secret my1stdbsecrets -o jsonpath='{.data.MYSQL_ROOT_PASSWORD}' | base64 -d
    echo -n 'cGFzc3dvcmQ=' | base64 –d

11. kubectl describe deployments.apps my1stdb

12. kubectl set env --from=secret/my1stdbsecrets deployment/my1stdb

13. kubectl describe deployments.apps my1stdb

14. kubectl get pods --selector app=my1stdb
```