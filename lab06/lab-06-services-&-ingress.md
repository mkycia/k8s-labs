# LAB-06

```
1. minikube addons enable ingress

2. kubectl create deployment nginx --image=nginx

3. kubectl expose deployment nginx --port=80

4. kubectl get svc nginx

5. minikube ssh
   curl http://<nginx-svc-ip>
   exit

6. kubectl edit svc nginx
(...)
  Protocol: TCP
  nodePort: 32000
type: NodePort

7. kubectl get svc

8. curl http://$(minikube ip):32000

9. kubectl get deployment nginx

10. kubectl get svc nginx

11. curl http://$(minikube ip):32000

12. kubectl create ingress nginx-ingress --rule="/=nginx:80" --rule="/hello=hello-app:8080

13. kubectl get ingress         # poczekać, aż wyświetli się IP węzła

14. kubectl describe ingresses.networking.k8s.io nginx-ingress

15. kubectl create deployment hello-app --image=gcr.io/google-samples/hello-app:2.0

16. kubectl expose deployment hello-app --port=8080

17. kubectl describe ingresses.networking.k8s.io nginx-ingress

18. curl http://$(minikube ip)

19. curl http://$(minikube ip)/hello
```