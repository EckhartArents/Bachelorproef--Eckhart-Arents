# GitHub container registery

Om mogelijk en alternatief te hebben voor de docker hub
Is om dit moment nog in beta en moet je manueel inschakelen
eerst met docker doen als leidraad
voor het pushen van docker naar github heb je een acces token nodig
docker login ghcr.io --username github-account
je moet zelf taggen aan de image of dat de repository ergens anders staat dan docker hub
en dan deze tag pushen
# nu eens in fedora met podman
## intermezzo: Fedora blog heeft net een post om containers kleiner te maken
https://fedoramagazine.org/build-smaller-containers/
de eerste stappen zijn zoals verwacht
de blog legt vooral uit wat je kan doen om je image kleiner te krijgen
zoals standaard inbegrepen dependenties verwijderen of een kleiner base image.
Vervolgens toont het ook hoe je met Buildah vanaf scratch een container kan maken
Buildah staat niet standaard geïnstalleerd
Toen ik het wou instaleren was eer en bestand conflict met de reeds geïnstalleerde podman
Uiteindelijk besloten om buildah terzijde te leggen
## Terug met de GitHub registery
Het pullen van de publieke werkt
Ook met podman kan je inlogen op de ghrc.io met je username en en api key
Dan analoog kun je ook je image tqggen en pushen naar github
## Pullen en draaien in minikube