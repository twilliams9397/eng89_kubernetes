# Kubernetes (k8)
- orchestration platform, controls behaviour of multiple containers
- where `docker compose` runs a few container, Kubernetes manages 100s/1000s
- can deploy multiple copies, load balance, self healing (manages containers going down automatically) 
- open sourced by google so publically available, used by ~70% of surveyed organisations in 2017
- other cloud providers (Azure, google cloud, AWS) run kubernetes based services as well
- managed services: resources managed by responsible team, can be interface or command line
- create a kubernetes cluster - platform to manage multiple running containers, e.g. docker containers
- advantages: self heal (auto spin up instance to replace any that go down), load balance between instances while self healing is performed, automated rollouts/rollbacks between working versions, auto scaling and bin packing, storage orchestration
- deployment replica sets, snapshots of same image and each pod has individual IP for connections/API