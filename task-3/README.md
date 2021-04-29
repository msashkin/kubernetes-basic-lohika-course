# Task 3

1. Create ConfigMap v1
   1. index.html (contains v1 specification)
2. Create ConfigMap v2
   1. index.html (contains v2 specification)
3. Create Deployment
   1. Container image: nginx:latest (exposed port 80)
   2. Replicas: 2
   3. Mount ConfigMap v1 to the container folder `usr/share/nginx.html`
   4. Create k8s Service to expose Deployment
   5. Provide a screenshot of the Service response (v1: browser, wget, curl etc.)
4. Update Deployment
   1. Mount ConfigMap v2 to the container folder `/usr/share/nginx.html`
   2. Provide a screenshot of the Service response (v2: browser, wget, curl etc.)
5. Scale Deployment to 3 replicas
6. Rollback Deployment version
   1. Check that Deployment created 2 ReplicaSets `kubectl get rs`
   2. Check Deployment history `kubectl rollout history deployment <deployment_name>`
   3. Rollback to the previous Deployment version `kubectl rollout undo deployment <deployment_name> --to-revision=<deployment_revision>`
