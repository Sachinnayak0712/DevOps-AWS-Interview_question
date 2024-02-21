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
	Auyomatic Bin Packing
		Kubernetes automatic bin packing works by intelligently scheduling containers onto nodes in a 	cluster, taking into account factors such as resource requirements, 				utilization, and availability
	Storage management 
	Self Healing
	Services discovery and load balancing
		Service Discovery enables efficient communication between these instances, while Load 	Balancing ensures that incoming traffic is distributed evenly across the available 			instances
	Automatic roolout and roolback
		Rollout: The ability to deploy lates minor version (bugfix, hotfix, minor feature, enhancement) without downtime. 
		Rollback: The ability to restore back the older working version in case something goes wrong.
	Horizontal Scalling
