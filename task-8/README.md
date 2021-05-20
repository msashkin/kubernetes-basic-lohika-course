# Task 8

1. Install helm binary (version 3)
2. Create helm chart with `helm create`
   1. Update config to use service type LoadBalancer
   2. Add resources requests and limits:
      1. CPU: 100m
      2. Memory: 200Mi
   3. Deploy chart to the cluster
   4. Find load balancer address (save it)
   5. Access service using load balancer address (browser, curl, wget, etc.)
   6. Provide screenshots
3. Check deployed Pod
   1. Enter deployed pod with `kubectl exec`
   2. Install curl with commands
      1. `apt-get update`
      2. `apt install -y curl`
   3. Run command `curl checkip.amazonaws.com`
      1. Provide returned address
   4. Access deployed load balancer with curl (`curl <load balancer address>`)
      1. Provide screenshot
   5. Check Pod’s logs
      1. Provide screenshot
