## readme

```bash
cd C:/h/a/f/software-architect-cource/labs/sprint-5/architecture-propdevelopment/Task5
> /architecture-propdevelopment/Task5 (architecture-propdevelopment)

kubectl run front-end-app --image=nginx --labels role=front-end --expose --port 80
kubectl run back-end-api-app --image=nginx --labels role=back-end-api --expose --port 80
kubectl run admin-front-end-app --image=nginx --labels role=admin-front-end --expose --port 80
kubectl run admin-back-end-api-app --image=nginx --labels role=admin-back-end-api --expose --port 80
service/front-end-app created
pod/front-end-app created
service/back-end-api-app created
pod/back-end-api-app created
service/admin-front-end-app created
pod/admin-front-end-app created
service/admin-back-end-api-app created
pod/admin-back-end-api-app created

kubectl apply -f .
networkpolicy.networking.k8s.io/allow-non-admin-pair created
networkpolicy.networking.k8s.io/allow-admin-pair created


kubectl run test-$RANDOM --rm -i -t --image=alpine -- sh
$ # wget -qO- --timeout=2 http://apiserver

winpty kubectl run test-$RANDOM --rm -i -t --image=alpine -- sh
/ # wget -qO- --timeout=2 http://apiserver
```
