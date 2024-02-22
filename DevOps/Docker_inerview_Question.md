# Beginner

What is Hypervisor and its type.\
What is virtualization.\
What is containerization.\
Difference between virtulization and containerization.\
What is docker.\
What is docker container.\
What are docker Images.\
What is docker hub.\
Docker Architecture.\
Docker file.\
Docker compose.\
Docker swarm.\
Docker namespace.\
Docker container life cycle.\
Docker machine.

# Intermidiate

## How to check docker server and client vesion.\
docker version


How to get the number of containers tunning pused and stopped.\
docker info


How to help for the docker.\
docker --help\
ex :\
if need to check on run command.\
docker run --help


Login into docker repository.\
docker login\
enter username and password

Use baseimage and make modification or personalize it.\
docker pull <image_name>

Create docker container from the image.\
docker run -it -d <image_name>

List all the running container.\
docker ps

Access a runnig container.\
docker exec -it <contianer_id> bash

How to start stop and kill a container.\
docker stop <contianer_id>\
docker start <contianer_id>\
docker kill <contianer_id> 

Can u user a contianer, edit it, and update it.\
docker commit <container id> <username/imagename>

Once u worker with an image how to push it to docker hub.\
docker push <username/image name>

Delete stoped container.\
docker rm <contianer_id> 

Delete an image from  the local storage system.\
docker rmi <image-id>

Build docker file.\
docker build <path to docker file>

Docker system prune.\
used to remove all netwok not in use, stopped container, dangling image, build cache


# Advanced

Will u lose ur data, when a docker container exits.
no it will be stored in disk, unless u explisitly delete the continer

Where all do u think docker is being used.
simplifying configuration
code pipeline mangement
developer productivity
pplication isolation
debbuging capabilities
multi-tenancy
rapid deployment

How docker is differne tfrom othe r containerization methods.
these are very easy todeploy in any cloud platform.
it can get more application running on the same hardware when comared to other technologies

Can i use json insted of yaml for my compose filein docker.
yes

How have you used docker in your previous position.

How for do docker containers scale? are there any requrement for the same.

What platform does docker run on.
ubuntu, fedora,ec2, ms azure

Identiy the status of container.
there are 5 states -> creating, running, paused, restarting, exited,dead

Can u remove paused container from docker.
no
docker has to be in stoped state

Can a container restart by itself.
no
restart is set to false

Is it better to directly remove the container using the rm command or stop the container followed by remove container.
its always better to stop the container and then remove it using remove command

Will cloud overtake the use of containerization.
no,  cloud services are giving a good fight

How many containers can run per host.
there can be as many conatainer as you wish per host
consider every container need storage space, CPU, memory which hardware needs to support
also should consider application size
continer are light weight but dependent on host operating system

Is it a good practive to run stateful application on docker.

Willdocker compose wait for the cunrrent continer to be ready to move to the running of the next services.
docker compse always runs in dependency order

How will u monitor Docker in Production.
using docker stats and docker enventsto monitit docker in production

Is it good practice to run docker compose in production.
yes, using docker compose in production is the best practival application of docker compose

What changes are expecte in your docker compose file while moving it to production.
remover volume bindings
binding to different ports on the host
specify a resart policy
add extra services like log aggregator

Have you used Kubernetes?if u  have , which would you prefer amongst Docker and Kubernetes.

Are you aware load balancing across containers and hosts? how does works.?
while using docker services with mutilple containers across different hostdu come acress the need to load balance the incoming traffic. Load balancing and HAProxy is basically used to balance the incoming traffic across different available(healthy) continers.

# General














