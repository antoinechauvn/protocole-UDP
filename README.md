# protocole-UDP
Découverte du protocole UDP

### Qu'est-ce que le protocole UDP?
UDP signifie User Datagram Protocol, et il s'agit d'un protocole de communication sans connexion. Le protocole UDP est une alternative au protocole TCP.
Lorsque le protocole UDP est utilisé pour transporter les données, il va envoyer les données d'un hôte source vers un hôte de destination, sans chercher à savoir si l'hôte de destination a bien reçu l'ensemble des données. Autrement dit, il n'y a pas de vérification des erreurs : si l'on envoie un fichier via UDP, on ne sait pas si l'hôte distant a reçu entièrement ce fichier ou s'il l'a reçu partiellement.
Puisque l'on ne vérifie pas que l'hôte distant a bien reçu les données, on économise des ressources, mais aussi du temps, donc le protocole UDP est plus rapide que le protocole TCP.

* Le protocole DNS pour la résolution des noms (même si TCP peut être utilisé dans de rares cas)
* Le protocole SNMP pour la supervision des équipements
* Le protocole NTP pour la mise à jour de la date et l'heure via le réseau
* Le protocole TFTP pour le transfert de fichiers simplifié

## Principe de fonctionnement
Le paquet UDP est encapsulé dans un paquet IP. Il comporte un en-tête suivi des données proprement dites à transporter.

![image](https://user-images.githubusercontent.com/83721477/168084857-d8ef09bb-2586-42c6-a429-8e943c313875.png)
L'en-tête d'un datagramme UDP est plus simple que celui de TCP :
![image](https://user-images.githubusercontent.com/83721477/168084960-b1b3833c-8e37-4286-93f0-5784aa440cd8.png)

