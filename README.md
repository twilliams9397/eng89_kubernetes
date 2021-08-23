# Kubernetes (k8)
![k8_cluster](k8_cluster.png)
- orchestration platform, controls behaviour of multiple containers
- where `docker compose` runs a few container, Kubernetes manages 100s/1000s
- can deploy multiple copies, load balance, self healing (manages containers going down automatically) 
- open sourced by google so publically available, used by ~70% of surveyed organisations in 2017
- other cloud providers (Azure, google cloud, AWS) run kubernetes based services as well
- managed services: resources managed by responsible team, can be interface or command line
- create a kubernetes cluster - platform to manage multiple running containers, e.g. docker containers
- advantages: self heal (auto spin up instance to replace any that go down), load balance between instances while self healing is performed, automated rollouts/rollbacks between working versions, auto scaling and bin packing, storage orchestration
- deployment of replica sets, snapshots of same image and each pod has individual IP for connections/API
- what problems, what challengs, what skillset, comms between tech/non tech - FA webinar
- challenge: already using microsft languages/service (azure, .net frameworks) so not compatible with k8 version
- analysts find it useful knowing the terms/processes for better understanding but havent always heard of the tech
- people dont always have the latest tech knowledge
- kubernetes can be expensive for smaller solutions, and needs prior understanding of containers, networking etc
- provider managed k8 services manage the master node for you, so there is no provisioning needed for the master node on launch, and managed services can vary from different providers
- in a self managed service there is more control over the cluster control, and can manage each layer component individually. there is also more control over deployment and administration of the clusters

## Setup
- after starting docker navigate to settings -> kubernetes and ensure it is enabled
- `kubectl` will give commands available and check if install was correctly done, and default clusters can be seen in the docker app
- `kubectl get service` will show the running services with info
- `kubectl get` can be `name_of_resource`, `node`, `pods`
- can use `kubectl describe pod_id` to see what is inside a pod, which are similar to containers
- can use docker desktop to view more container details and see what is running

## Prerequisites/task
- ensure all required ports for app are available - 3000, 80 and 27027 for sparta node app
- create k8 deployment file called nginx_deployment.yml
- use default nginx image
- create 2 replicas of this deployment
- `kubectl create -f file_name.yml` will run the deployment file
- `kubectl get deployment` or `deploy` will list what has been deployed and is running






