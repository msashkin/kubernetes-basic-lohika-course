# Task 1

1. Create k8s secret with 2 values:
   1. username
   2. password
2. Create k8s pod
   1. container image: ealen/echo-server (exposed port 80)
   2. use values from the secret as environment variables
3. Create k8s service to the exposed pod
4. Provide a screenshot of the service response (browser, wget, curl, etc.) using `kubectl proxy` command:
   1. `kubectl proxy`
   2. `curl http://127.0.0.1:8001/api/v1/namespaces/<namespace_name>/services/<service_name>/proxy/`
