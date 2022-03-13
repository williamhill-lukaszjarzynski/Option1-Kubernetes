# Option1-Kubernetes
The Task

Your task is to create a repo in github and solve below problem

1. CREATE 
   
   # a kubernetes deployment, 
   # svc - service, 
   # hpa - horizontal pod autoscaler, 
   # pdb - pod disruption budget service account 
   
   in kubernetes cluster. (can be PaaS/MINIKUBE)
   
2. Deployment needs a secret with name "API_KEY"
3. Mount this secret in deployment
4. "API_KEY" should be a environment variables within the container when container starts inside a pod
5. "API_KEY" env variable is not used yet in app, but we want to see the approach

# Acceptance criteria

## You must provide your code in full with kubernetes manifests or pipelines or scripts

## You must use either public cloud(AWS, GCP, Azure) or Minikube to run the above manifests file

## You do not need to provide access to the cluster in public cloud, only the code

## Your code is clean and readable

## You must document any steps that are not automated in the README.md

## You must have dedicated service account for deployment

## You must have NodePort Type of service for application

## You must have Minimum 2 pods always up and running

## You must have only 1 pod unavailable during Rolling Update of Deployment

# Assumptions

1. Can use any open-source tools/language to solve problem
2. Create extra code if needed like infra(terraform, scripts) etc in same repo
3. Choose simple applications from internet e.g. nginx, httpd

# Bonus

1. Deployment container is scanned before getting deployed. If severity is high, pipeline should fail
2. Container in Pod, should not be running as root
3. Provide any code that you required to accomplish this task
4. You must document any steps that are not automated in the README.md

