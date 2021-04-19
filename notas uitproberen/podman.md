# Podman 

Podman in een fedora vm

Podman is een veel belovend alternatief

De fedora help pagina's raden podman aan als alternatief voor Docker

Eenvoudig commando voor home fedora installatie, die niet eens nodig is want de Geïnstalleerde fedora zegt dat het al geïnstalleerd is

Commando's van Polman lijken goed op die van docker

We instaleren ook Visual studio code om makkelijker aanpassingen te doen in bestanden dan met vi of vim.

We proberen eens na te doen in podman wat lukte in docker op windows

Dus ook met [https://github.com/docker/getting-started/tree/master/app](https://github.com/docker/getting-started/tree/master/app) Als start app

# Eerst het builden

Podman gebruikt buildah voor het effectief te builden maar buildah moet niet apart geïnstalleerd zijn

De file voor het builden is equivalent met de dockerfile op naam na, het mag zowel dockerfile als contiainerfile heten.

Om verwariging te vermijden zal ik het contiainerfile noemen

Visual studio gebruikt de zelfde extenties ook hier mogelijk

Podman help zegt dat de containerfile automatisch in de huidige map gezocht word mar dat leek niet het geval dus heb ik het Manuel gespecifieerd waardoor de built wel lukte.

Het builden en opstarten is volledig analoog gelukt

Stopen is ook met id of zoals de help pagina's van podman uitleggen ook mogelijk met de (gegenereerde) naam

Nu een simpele volume toevoegen aan de app dit gebeurt ook analoog

# Nu een kijken of het me ook lukt om het in twee delen op te splitten voor de databank

Podman heeft pods voor meerdere samen hangende containers

Het via comand line verbinden lukt me niet, deels omdat de exlorre die het docker voorbeeld gebruikt enkel voor docker netwerken werkt En netwerk configuratie is iets anders voor pods

via comand line verbinden lukt me niet is er mogelijkeih om het te doen via configuratie bestanden
# podman compose

Om het substitueren van docker verder te zeten bestaat er ook Podman compose
https://github.com/containers/podman-compose
is wel nog onder active development

bij het opstarten met een volume geeft de laatste stabiele release een fout, dus instaleer ik de dev versie die deze fout zou moeten opgelost hebben

het nabootsen van het compose gedeelte van de docker todo app tutorial geeft veel warnings en sommige errors met podman compose.

Podman zegt dat de pod met de containers aan het runnen is maar het lukt me niet op het via de ingestelde port te bereiken

Is dit soort verbinden van containers zelfs nodig? Is dit niet ook met kubernetes te doen?