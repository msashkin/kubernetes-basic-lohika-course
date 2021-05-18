# kubernetes-basic-lohika-course

Kubernetes Basic Lohika Course

Create a secret imperatively:

```sh
kubectl create secret generic my-creds --from-literal='username=msashkin' --from-literal='password=P@ssw0rd'
```

Create a configmap imperatively:

```sh
kubectl create configmap my-configmap-v1 --from-file=configmaps/v1/
```

Apply all resources from folder:

```sh
kubectl apply -f ./
```

Delete all resources from folder:

```sh
kubectl delete -f ./
```
