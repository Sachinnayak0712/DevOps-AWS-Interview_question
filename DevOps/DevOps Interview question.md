# What is Docker? 
Docker is a tool by using which, we create containers in less time. Docker uses light weight OS in the form of docker images that we will get from docker hub. Docker is open source now.
Docker image is light weight OS provided by docker company. We can get any type of docker image form docker hub.

# What is virtualization? 
Logically dividing big machine into multiple virtual machines so that each virtual machine acts as new server and we can deploy any kind of applications in it.
Virtualization relies on hypervisors and complete OS instances, providing strong isolation and compatibility with diverse operating systems.

# What is Containerization
containerization runs a single OS instance, with multiple user spaces to isolate processes from one another.
Containerization, on the other hand, leverages lightweight containers and shared OS, offering increased agility, portability, and scalability


# K8 
Kubernetes, also known as K8s, is an open-source system for automating deployment, scaling, and management of containerized applications

# Feature of K8
	1) Automatic Bin Packing
		Kubernetes automatic bin packing works by intelligently scheduling containers onto nodes in a 	cluster, taking into account factors such as resource requirements, 				utilization, and availability
  
	2) Storage management 
 
	3) Self Healing
 
	4) Services discovery and load balancing
 
		Service Discovery enables efficient communication between these instances, while Load 	Balancing ensures that incoming traffic is distributed evenly across the available 		instances
  
	5) Automatic roolout and roolback
		Rollout: The ability to deploy lates minor version (bugfix, hotfix, minor feature, enhancement) without downtime. 
		Rollback: The ability to restore back the older working version in case something goes wrong.
  
	6) Horizontal Scalling

 # K8 Architecture
![1692026023846](https://github.com/Sachinnayak0712/DevOps-AWS-Interview_question/assets/66566069/15d2c3b3-e667-4463-a381-732767bfd95e)
# Kubernetes Archetecture
There are 2 main component 
	1) Master Node(Controle Plane) -> manages the worker nodes
 
	2) Worker Node -> Here Docker Engine is running

Master node -> 
	1) API server
 
	2) Scheduler
 
	3) Controller Manager
 
	4) etcd
 
Worker nodes -> 

	1) Kublet
 
	2) Proxy
 
	3) podes
 

## Master Node
Control Plane Components
API server - The API server is a component of the Kubernetes control plane that exposes the Kubernetes API. It is like an initial gateway to the cluster that listens to updates or queries via CLI like Kubectl. Kubectl communicates with API Server to inform what needs to be done like creating pods or deleting pods etc. It also works as a gatekeeper. It generally validates requests received and then forwards them to other processes. No request can be directly passed to the cluster, it has to be passed through the API Server.

Kube-Scheduler
When API Server receives a request for Scheduling Pods then the request is passed on to the Scheduler. It intelligently decides on which node to schedule the pod for better efficiency of the cluster.

Kube-Controller-Manager
The kube-controller-manager is responsible for running the controllers that handle the various aspects of the cluster’s control loop. These controllers include the replication controller, which ensures that the desired number of replicas of a given application is running, and the node controller, which ensures that nodes are correctly marked as “ready” or “not ready” based on their current state.

etcd 
It is a key-value store of a Cluster. The Cluster State Changes get stored in the etcd. It acts as the Cluster brain because it tells the Scheduler and other processes about which resources are available and about cluster state changes.


## Worker Node
Node Components
These are the nodes where the actual work happens. Each Node can have multiple pods and pods have containers running inside them. There are 3 processes in every Node that are used to Schedule and manage those pods.

Container runtime
A container runtime is needed to run the application containers running on pods inside a pod. Example-> Docker

kubelet
 kubelet interacts with both the container runtime as well as the Node. It is the process responsible for starting a pod with a container inside.

kube-proxy
It is the process responsible for forwarding the request from Services to the pods. It has intelligent logic to forward the request to the right pod in the worker node.


