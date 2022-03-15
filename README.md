# Option1-Kubernetes
The Task

http://www.yamllint.com/ - The YAML Validator

Your task is to create a repo in github and solve below problem

# All manifests file under:   https://github.com/williamhill-lukaszjarzynski/Option1-Kubernetes/tree/master

Each config file has 3 parts: metadata, specification, status.

1. 
   
   # a kubernetes deployment,  - YAML configuration file, where replicas: 2      - 
   https://github.com/williamhill-lukaszjarzynski/Option1-Kubernetes/blob/master/nginx-deployment-secret.yaml
   
2. Deployment needs a secret with name "API_KEY"
3. Mount this secret in deployment
4. "API_KEY" should be a environment variables within the container when container starts inside a pod     -  env with name: "API_KEY"
5. "API_KEY" env variable is not used yet in app, but we want to see the approach                          - I put the code into repo to use it,bu we can have it 
                                                                                                              as object ConfigMap to reference to file
   
   
   
   
   # svc - service, 
   https://github.com/williamhill-lukaszjarzynski/Option1-Kubernetes/blob/master/nginx-service.yaml
   
   
   # hpa - horizontal pod autoscaler, 
   
   
   # pdb - pod disruption budget service account 
   
   in kubernetes cluster. (can be PaaS/MINIKUBE)
   
   # MINIKUBE            - ALL OBJECTS in K8S CLUSTER from manifests - yaml configuration files:
   
     kubectl get all

   



kubectl get secret
kubectl get pod
kubectl describe pod nginx-deployment-secret


# Acceptance criteria

## You must provide your code in full with kubernetes manifests or pipelines or scripts (X)

## You must use either public cloud(AWS, GCP, Azure) or Minikube to run the above manifests file (X)

## You do not need to provide access to the cluster in public cloud, only the code (X)

## Your code is clean and readable (X)

## You must document any steps that are not automated in the README.md (X)

## You must have dedicated service account for deployment (x)       - lukasz

## You must have NodePort Type of service for application (X)       - type: NodePort

## You must have Minimum 2 pods always up and running   (X)         - ReplicaSet=4

## You must have only 1 pod unavailable during Rolling Update of Deployment (X)  - type: RollingUpdate with parameter for strategy

# Assumptions

1. Can use any open-source tools/language to solve problem
2. Create extra code if needed like infra(terraform, scripts) etc in same repo
3. Choose simple applications from internet e.g. nginx, httpd

# Bonus

1. Deployment container is scanned before getting deployed. If severity is high, pipeline should fail
2. Container in Pod, should not be running as root
3. Provide any code that you required to accomplish this task
4. You must document any steps that are not automated in the README.md

-------------------------------------------------------------------------------------------------------------------
   
   
   
   


