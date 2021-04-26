ik had de ubuntu vm tog staan dus kan deze eve goed voor iets anders benutten

# Docker in Ubuntu

Instaleren van de Docker engine volgens de docs

Basis install van de meest recente versie werk

De Docker deamon werkt op een socket die enkel door de root aangesproken kan worden

Waar dat podman rootles werkt, dit is dus al een zekere risico die docker toegeeft.Er bestaat een onstabiele omleidingen hievoor.

Om zelf niet altijd sudo uit te voeren volg ik de post installatie stappen om mijzelf aan een gerechtige  docker usergroep toe te kenen in Ubuntu

Op Ubuntu en Debian start Docker automatisch bij boot, voor andere distro’s zou je zelf moeten instellen of het mag starten bij boot

Het herdoen van een basis container app is het zelfde als native op mijn windows met de uitzondering dat ik images niet kan starten/stoppen/verwijderen via de desktop dashboard maar de achterliggende commando’s blijven hetzelfde

De docker compose moet echter nog apart gedownload worden

Hiervoor volgen we de instructies van de docker docs

De installatie is nog vrij eenvoudig

En dan met compose up en down lukt he top de gebundelde containers te verbinden en te draaien

Zonder de desktop app is het echter wel iets moeilijker om te zien welke images er zijn en draaien tussen de gewoonde docker engine en de docker compose omgeving

Ook voor docker is images = image ls, Maar docker compose heeft enkel images om de images te tonen

Zonder de desktop applicatie is er ook geen gebundelde kubeernetes omgeving
Dus Minikube kunnen we gebruiken maar het verschil met de podman versie zou enkel liggen in de driver die het gebruikt, en minikube zoekt standaard naar de docker en is met docker het meest stabile. we pakken eens het meest toegankelijke alternatief om uit te testen:

# hashicorp Nomad

Downloaden van de executabele van de site en zelf juist zetten volgen de instellingen van een Linux systeem
(Gelukig herriner ik me nog genoeg om te weeten hoe)

Voor container runtimes heeft nomad standaard ondersteuning voor docker, er bestaat een plug-in voor podman maar die is op dit moment lichtjes veroudert en vergt veel bijkomende configuratie van nomad

Volgen van een nomad tutorial

Eerst een agent opstarten de terminal die dit draait moet open blijven tijdens de dev omgeving die we aan het gebruiken zijn

Voor configuratie berust het op hasicorp configuration language (json kan ook maar is aangeraden enkel voor gegeneerde bestanden json te gebruiken)

We runen eens de example job

De naam voor de “.nomad” woord genomen als naam voor de job

Dit vorbeeld is een kleine redis container

Vervolgens is de config van deze job aanpassen

Visual studio code heeft een extensie om HCL te ondersteunen

We passen aan hoeveel instanties er tegelijkertijd uitgevoerd moeten worden

Eerst de verandering plannen en dan de job uitvoeren

Nu ook eens de versie van de container aanpassen

De update word niet gelijk tijdig uitgevoerd en verloop gefaseerd

Nomad heeft ook een web interface/dashboard die standaard op localhost poort 4646 gehost woord

Via de web interface kan je ook de status bekijken

Naast specifieke jobs kan je ook de clients en servers status bekijken

Veel van de command line functies kunnen hier ook gedaan woorden vb een job starten of stopen, maar in tegensteling tot  de kubernetes dashboard zegt het niet wat dat de equivalente command line instructie is.

Het stopen van een job en het beëindigen van de dev instantie lukken ook zoals uitgelegd

Nomad lijkt wel wat op k8. maar het laat ook toe om java of zelfs gewoon binairy executable taken uit te voeren via je ochestration omgeving.

de eigen configuratie taal ten opzichte van Yaml is mischein wel nog een minpunt