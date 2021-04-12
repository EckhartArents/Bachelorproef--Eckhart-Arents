# docker
docker als controle en beginpunt 
er zijn ook regelmatig screenshot genomen en bewaard maar die zitten niet in de git op dit moment

# WSL2 

Werken met docker op mijn laptop

We gaan voor de docker dektop versie met linux containers dus nood aan WSL2

Wsl2 enablen volgens de windows hulp

[https://docs.microsoft.com/nl-nl/windows/wsl/install-win10](https://docs.microsoft.com/nl-nl/windows/wsl/install-win10)

mijn versie is net goed genoeg voor de subsytem

hoe we dit weer deactiveren is en zorg voor later

[https://docs.docker.com/docker-for-windows/install/](https://docs.docker.com/docker-for-windows/install/)

# docker desktop instaleren

De desktop instaler voor windows geeft de optie om wsl 2 voor te bereiden, ik weet niet of dat dit de stappen die ik eerder gedaan heb van de feature  aan te zetten en up te daten doet of juist alleen de juiste linux distributie aanmaakt in wsl.

Instaltie vraagt om uit te loggen

Docker desktop start met een eigen kleine tutorial die pullen, builden, opstarten en pushen uitlegt.

Ik had een probleem bij het publishen, poort 80:80 is al door iets gebruikt. ik denk van iets uit web 3 en de dot net uitvoerende omgeving 

De docker desktop geeft toegang tot een betere interface voor overzichten maar de opstart en aanmaak is nog steeds met cli.
# betere tutorial volgen
We volgen de uitgebreide tutorial van docker

https://docs.docker.com/get-started/02_our_app/

We gebruiken Visual studio code per aanbeveling en extensies

Maken een image en runen het op localhost deze keer op een poort die nog niet gebruikt wordt,

Firewall komt tussen en waarschuwt,

Aanpassingen in de bron bestanden moeten eerst weer gebuild worden en en hiervoor moeten we de oude removen

Nieuwe opstarten en kijken of het werkt nog steeds werkt

(Eens pushen en proberen met play with docker)

Alle gegevens gaat verloren als de container stopt dus Db persisten

Een simple volume toevoegen werkt ook zoals uitgelegd

Bind mounts toevoegen

Moet met powershell; cmd is niet voldoende

Het op deze manier doen heeft de db verwijdert

Nu is het de twee verbinden door een netwerk te starten in docker

Concet using nicloa netshoot

We binden de dev databank en haalen de records eens op

Best practises scan

Door de volgorde aan te passen word de build veel sneller
# eerste bedenkingen 
Een eenvoudige 2 containers app met docker desktop (meer bepaald de engine en composer) lukt en is niet al te moelijk.
voor Linux zou je de huidige status niet in een desktop applicatie zien en moet je apart de engine en composer instaleren. als alles toch voornamelijk uitgelegd word aan de had van de cli zal er weinig verschil zijn. 
echter hoe je acteraf wsl2 uitschakelt is een mogelijk en probleem
kubernetics en swarl gebruiken doe ik nadat ik een par andere runtimes uitprobeer, voornamelijk eerst podman en zien in andere vms wat er werkt.