
# first party sites
directly or indirectly provides software for contairer oparation.

## docker family ("standard"):
https://www.docker.com/
Has runtime (docker engine), Cluster management and deployment (docker swarm & docker datacenter) , docker hub ( container images)
images based of Open Container Initiative (https://opencontainers.org/)
werken alemaal met elkaar en ondersteunt ook kubernetics
ook account nodig
### Docker Desktop
engine applicatie voor mac en windows, linux vraagt specifiek engine te downloaden
komt met kubernetics server

### Docker engine
speciefieck voor het draaien van docker containers
versies voor Azure, aws, Fedora, Ubuntu, centOS, Debian  

### Docker Hub 
een online repository voor images van containers
gratis account heeft geen private repsototries , alles zou publiek zijn

### Docker swarm
is voor clusters van engines
standaart met de engine gebundelt
via comand line
multi node swarms niet mogelijk op mac en windows 

### docker compose
de tool om merdere contaiers te runnen
standaart in de desktop versie
manueel te downloaden voor linux en servers
via comand line

### dockercraft
https://github.com/docker/dockercraft
docker in minecraft
bezienswaardigheid en niet actief sinds 2018

## kubernetics (orchestration)
https://kubernetes.io/
go to for orchestration
containers verbinden over merdere computers
miniku is de go to voor locaal


### minikube
https://minikube.sigs.k8s.io/docs/start/
"minikube is local Kubernetes, focusing on making it easy to learn and develop for Kubernetes."
via comand line
nood aan 2 cpu's
werkt met docker, podman, CRI-O
alle os
kan in de kuberetics dashboard gebruikt worden

## CRI-O (runtime)
https://cri-o.io/
for kubernetics
based on OCI
LIGHTWEIGHT 
alle OCI compliant containers van repositories
enkel voor linux distributies
comand line

## Containered (runtime) 
https://containerd.io/
based on OCI
voor linux en windows
ook alle OCI compliant containers van repositories
comand line

## Podman (runtime )
https://podman.io/
posibly promising alternative
remote client voor een linux box op windows of mac
ondersteunt  veel van de linux distrubuties
command line

## kata containers (VM like runtime)
https://katacontainers.io/
maybe best to stick to true containers
linux distributies
werkt met kubernetics, cri-o containered


## linux containers (engine en orchestration)
https://linuxcontainers.org/
container close to system but less overhead
voor linux distributies
heeft enkel client versie voor windows en mac, dus deze zijn gelimiteerdd tot 1 machine
command line

## mesos (orchestration)
http://mesos.apache.org/
not only containers
voor linux distributies, mac (el captain en sierra), en windows
werkt met docker
heeft ook een engine 

### Marathon
https://mesosphere.github.io/marathon/
werkt bovenop apache mesos

## Nomad (orchest)
https://www.nomadproject.io/
containers and not containerd support
linux, mac en windows
eigendom van hashicorp


## envoy (service mesh)
https://www.envoyproxy.io/
networking and observation
probably not relevant

## pouch container (engine)
https://pouchcontainer.io/
owned by Alibaba

## Github Container Registry
https://docs.github.com/en/packages/guides/about-github-container-registry
Beta versie , nood aan feature preview
zowel dokker als algemeen OCI


## GitLab Container Registry 
https://docs.gitlab.com/ee/user/packages/container_registry/
project of team gebonden repository voor container images
zowel dokker als algemeen OCI


# smaller providers
startups or just github repo's

## balena-engine
https://github.com/balena-os/balena-engine
last stable realese DEC 2019, doesn't seem very active, IOT containers engine

## flockport
https://www.flockport.com/
Startup, small, possibly died in 2019? intended to be a complete package for containers?

## Rexray
https://github.com/rexray/rexray
last stable release jan 2019, seems dead, was intedned for container storage orchestration

## eliot
https://docs.eliot.run/
still in alpha, intended for IOT

# vernoemt in papers 

## Chroot
comando van linux de oudeste vorm van contanerisation

## Fleet
was van CoreOS, beindigt in 2017 nu in redhat

## BSD Jailes
specifiek containers en virtualisatie voor de BSD os
had ik nog nooit van gehoord

## Solaris Zones & Containers
specifiek voor de solaris os

## AIX Workload Partitions
voor AIX os van IBM

## CoreOS’s Tectonic
was vore CoreOS
nu geintegreert in openshift

## Rancher Labs' Rancher
https://rancher.com/
extra stap voor met kubernetics en docker te werken

## Open VZ
https://openvz.org/
open source 
enkel voor linux
vm+containers

## Sandboxie
https://sandboxie-plus.com/
nu open source
site ziet er verdacht uit 
is voor vm's

## YARN
deel van hadoop apache, moelijk info over te vinden

## Joyent Triton
https://www.joyent.com/triton/compute
vooral voor cloud
een extra bovenop docker of kubernetics

## Cloudify
https://cloudify.co/
orchestrtion over merdere clouds minder praktish van toepassing 

## DC/OS
https://dcos.io/
server os 
nauw verbonden met mesos

## aurora
was ook van apache
is in 2020 beinigt

# Cloud support
cloud solutions

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

## Windows containers
hun uitleg werkt gewoon met docker dus geen eigen alternatief
een andere runtime van containers genaamt Windows containers
enkel op windows servers of Professional/Enterprise editions

## azure
again kubernetics support
https://azure.microsoft.com/en-us/services/kubernetes-service/
and a more vauge container support 
https://azure.microsoft.com/en-us/services/container-instances/

## Azure Container Registry
Container Registry als deel van de cloud aanbod

# red hat
heeft account nodig voor alles
https://www.redhat.com/

## openshift
https://www.openshift.com/
container application platform
suported by AWS, google, Azure (platform as a service)

https://www.openshift.com/try
also localy posible? (need account to see)
enkel Red Hat Enterprise Linux (RHEL), Microsoft Windows, and macOS

## OpenShift Container Storage
cloud container repository

## Red Hat Quay
https://www.openshift.com/products/quay
een andere container storage

## openstack (orchestration)
https://www.openstack.org/
has local runing posibilites maar zegt veel systeem aanpasingen te doen
drop

## rkt 
https://www.openshift.com/learn/topics/rkt
application container engine, moved to Cloud Native Computing Foundation (CNCF)
github zegt dat het gearchiveerd is

# google
has support in cloud
https://cloud.google.com/containers

## borg & Omega
de oude cluster management tools van google

## Google Container Engine
hun naitive cloud onderstuning voor kubernetics en docker

## Container Registry
deel van hun cloud anbeiding
