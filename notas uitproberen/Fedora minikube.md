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

hievor zal ik ook nog eens kijken hoe ik met podman een image push naar of te wel docker of github.

# Pullen van GitHub en tonen in minikube en kubernetes
Publieke images kan kubernetes van overal pullen,  voor private heeft het ondersteuning voor docker hub en google Cloud registery.

Ik probeer eens met de dashboard een pod te starten, hier beeft het de optie op het met een form te doen

Kubernetes geeft geen fout bij het pullen van de publieke repository

Minikube geeft zelf andere ports aan je pods via services.

## Eerst lokaal pullen en dan deze draien in kubernetes?
Sinds dat prive niet ondersteunt is zou ik willen testen of dat een lokaal bestaande image gebruikt kan worden.
Een voor de hand liggende manier om lokaal bewaarde images te pakken en te draaien heeft kubernetes niet. Ze stellen voor om hoofdzakelijk te werken met open source images zodat je niet meteen iets te verbergen hebt of als er toch iets gevoelig is het op een lokaal netwerk achter een firewall publiek te zetten om zo op te halen.
