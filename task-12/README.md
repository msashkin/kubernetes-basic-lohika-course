# Task 12

Based on the task 3 of the workshop 2

1. Based on the different `index.html` content from the task 3 create 2 deployments and 2 services with different content (ver1 and ver2)
   - configmap: ver1
   - deployment: ver1
   - service: ver1
   - configmap: ver2
   - deployment: ver2
   - service: ver2
2. Create ingress with path-based routing similar to the example
   - `/<STUDENT NAME>/v1` - to access service ver1
   - `/<STUDENT NAME>/v2` - to access service ver2
   - Don't forget to add annotation to the ingress:
     - `nginx.ingress.kubernetes.io/rewrite-target: /`
   - Deploy configurations to the cluster
   - Try to access deployed applications using URLs:
     - `http://a91f596e4f5074462bcdf247997bc564-c1069da4d48722e6.elb.us-east-2.amazonaws.com/<STUDENT NAME>/v1`
     - `http://a91f596e4f5074462bcdf247997bc564-c1069da4d48722e6.elb.us-east-2.amazonaws.com/<STUDENT NAME>/v2`
   - Provide screenshots
   - Cleanup resources
