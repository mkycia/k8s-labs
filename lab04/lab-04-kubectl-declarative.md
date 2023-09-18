# LAB-04

```
1. kubectl create deploy nginx --image=nginx --dry-run=client -o yaml > nginx_deployment.yaml

2. vim nginx_deployment.yaml              # dodanie labelki tier: frontend
                                          # zmiana ilości replik na 2

(...)
metadata:
  labels:
    tier: frontend
(...)

spec:
  replicas: 2
(...)  

3. kubectl apply -f nginx_deployment.yaml

4. kubectl describe deployment nginx      # proszę zauważyć, że: StrategyType: RollingUpdate

5. vim nginx_deployment.yaml              # ustawiamy spec.strategy na type: Recreate
(...)
spec:
  strategy:
      type: Recreate
(..)

6. kubectl apply -f nginx_deployment.yaml

7. kubectl describe deployment nginx      # proszę zauważyć, że: StrategyType: Recreate

```