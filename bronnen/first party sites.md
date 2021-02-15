
# first party sites
directly or indirectly provides software for contairer oparation.

## docker family ("standard"):
https://www.docker.com/
Has runtime (docker engine), Cluster management and deployment (docker swarm & docker datacenter) , docker hub ( container images)
images based of Open Container Initiative (https://opencontainers.org/)

## kubernetics (orchestration)
https://kubernetes.io/
go to for orchestration

### minicube
https://minikube.sigs.k8s.io/docs/start/
"minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes."

## CRI-O (runtime)
https://cri-o.io/
for kubernetics
based on OCI

## Containered (runtime) 
https://containerd.io/
based on OCI

## Podman (runtime )
https://podman.io/
posibly promising alternative

## kata containers (VM like runtime)
https://katacontainers.io/
maybe best to stick to true containers

## linux containers (engine en orchestration)
https://linuxcontainers.org/
container close to system but les overhead

## mesos (orchestration)
http://mesos.apache.org/
not only containers

## Nomad (orchest)
https://www.nomadproject.io/
containers and not containerd support

## openstack (orchestration)
https://www.openstack.org/
has local runing posibilites

## envoy (service mesh)
https://www.envoyproxy.io/
networking and observation
probably not relevant

## pouch container (engine)
https://pouchcontainer.io/
owned by Alibaba


# smaller providers
startups or just github repo's

## balena-engine
https://github.com/balena-os/balena-engine
last stable realese DEC 2019, doesn't seem very active, IOT containers engine

## flockport
https://www.flockport.com/
Startup, small, possibly died in 2019? intendet to be a complete package for containers?

## Rexray
https://github.com/rexray/rexray
last stable release jan 2019, seems dead, was intedned for container storage orchestration

## eliot
https://docs.eliot.run/
still in alpha, intended for IOT

# Cloud support
specificly cloud solutions

## amazon aws
https://aws.amazon.com/
has Amazon Elastic Container Service for containers
also has direct suport for kubernetics and openshift

## cloud foundry (platform as a service)
https://www.cloudfoundry.org/
has its own kubernetics based suite
provided by ibm, SAP, Atos cloud solutions

## digital ocean 
https://www.digitalocean.com/
cloud hosting platform, with kubenetics support

## instana
https://www.instana.com/
IBM bought cloud Paas
to wide a net

# microsoft 
https://docs.microsoft.com/en-us/virtualization/windowscontainers/about/
visual studio and code offer support for containers
doesn't mention OCI but support docker hub

## azure
again kubernetics support
https://azure.microsoft.com/en-us/services/kubernetes-service/
and a more vauge container support 
https://azure.microsoft.com/en-us/services/container-instances/

# red hat
https://www.redhat.com/

## openshift
https://www.openshift.com/
container application platform
suported by AWS, google, Azure (platform as a service)

also localy posible? (need account to see)

## rkt 
https://www.openshift.com/learn/topics/rkt
application container engine, moved to Cloud Native Computing Foundation (CNCF)

# google
has support in cloud
https://cloud.google.com/containers