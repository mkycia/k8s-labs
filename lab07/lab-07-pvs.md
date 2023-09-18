# LAB-07

```
1. kubectl create -f pvs-pod.yml

2. kubectl get pods 

3. kubectl describe pods pvs-pod 		      # proszę zauważyć, że to jest multi-container pod

4. kubectl exec -it pvs-pod -c c1 -- touch /data1/test

5. kubectl exec -it pvs-pod -c c2 -- ls -l /data2
```