# Fedora minikube

https://minikube.sigs.k8s.io/docs/start/

omdat het in ubuntu niet lukte doek ih maar met fedora waar ik weet dat podman al geinstaleerd is.

Ook hier niet vergeten 2 virtuele CPU toe te kennen die minikube wilt

minikube zegt cri-o aan te raden bij podman https://minikube.sigs.k8s.io/docs/drivers/podman/

bij het opstarten van minikube geeft het een gekende fout die ook bij de driver uitleg voor podman verholpen wordt door configuratie van je systeem aan te passen.

Het opstarten van de minikube duurt een tijdje,  minikube komt met een kubenetes dashboard

moet  wel nog zelf kubectl instaleren om met de cluster te praten https://kubernetes.io/docs/reference/kubectl/overview/

het volgen van de minikube start up lijkt voor de rest te werken,

ook de dasboard interface help om al eens te scalen of andere comandos en vermelt telkens de equivalente command line methode


laten we nu eens een wordpres proberen maken analoog als dat niet lukte met docker
https://kubernetes.io/docs/tutorials/stateful-application/mysql-wordpress-persistent-volume/
braaf de stapjes volgen en het werkt

zelfs met maar 4gb aan ram geheugen lijkt het te werken in de Fedora VM en heeft het geen merkbare nadeelige belasting

ook gebruert de coniguratie in de yaml files en moet je niet zelf verbindingen leggen via CLI( wat ik moelijker vind)

ik moet wel nog eens kijken hoe ik precies een egeigen gemaakte image in de minikube kubernetes krijg

hievor zal ik ook nog eens kijken hoe ik met pod,an een image push naar of te wel docker of github.
