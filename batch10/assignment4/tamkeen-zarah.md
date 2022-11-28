## Describe Architecture of Kubernetes 

An opensource containerization tool

Kubernetes Architecture has following components:

### - Master nodes
### - Worker nodes

Master Node has further following componets:

### - API Server

    - Responsible for all the tasks to run on a Kubernetes cluster


### - Scheduler

    - Schedules the tasks to slave node in the form of pods and services

### - Controller Manager

    - Manages the Kubernetes cluster
    - Matches the current sate with desired state  

### - ETCD

    - The database which stores all the key values of a cluster
    
Worker Node has further following componets:

### Container runtime

  - To run and manage containers on the worker node

### Kubelet

  - An agent which communicates with the Master node and executes on worker nodes
  - Ensures if the containers on Pod are running and healthy

### Kube-proxy

  - runs on each node
  - ensure that the services are available
  - kube-proxy sets up the routes

### Pods
  - one or more containers that logically go together. Pods run on nodes. Pods run together as a logical unit. So they have the same shared content. They all share the same IP address but can reach other Pods via localhost, as well as shared storage. Pods don’t need to all run on the same machine as containers can span more than one machine. One node can run multiple pods.
