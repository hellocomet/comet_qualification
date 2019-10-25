# Comment peut-on créer le système de gestion des bombes atomiques Français (sous-marin, bunker...,) ? le président veut pouvoir le suivre cela facilement 
> et tirez Mouhahahaha ! 

## Introduction
Ce scénario change des scénarios classiques (youtube, slack...). 
C'est le côté délirant qui déstabilise. donc il doit être fun ! 

Il amène des questions stratégiques complexes : 
- gestion de la géolocalisation
- gestion des flux de données (position des bombes)
- gestion de la sécurité (...captain Obvious)
- gestion du temps réel
- gestion de front adapté au président
- gestion de backend (récupération de données, aggrégat des résultats)
- Structure de l'équipe pour monter le projet
- modèle de données simple
- Test coverage à 100%


## Drill Downs

**Les bombes**

+ Comment tu greffe la géolocalisation ? (simplification : raspberry PI)
+ Quelles données envoies tu ? (Géolocalisation, Geohash...)

**Flux de données**

+ Comment envoies tu les données ? pour 10 bombes ? pour 4000 bombes ? (MQTT, par satelitte, websocket, wifi...)
> on va parler de bytes, scalabilité, socket...

**l'infra**

+ Comment construis tu ton infra ? datacenter...
> pas d'aws ou de google mais on peut s'en inspirer

+ Comment gères tu le flux arrivant ? loadbalancer.... 

> reprendre la question sur les flux de données et donc la taille des transferts de données

**Backend**

+ Que vas tu utiliser sur le backend ? LAMP, Nodejs,... ? 
+ Quel framework ? 
+ Quel langage ? 
> Pensez à suggérer la techno utilisée dans l'historique du candidat

+ Comment vas tu gérer le cache et l'afflux de données ?
Qui porte la sécurité ? Le loadbalancer ou les instances back ... ?  

+ Quelles librairies utilises tu ? (express+....)
+ Quelles structures d'application appliques tu ? 
+ microservice ou monolithique ? 

**La sécurité**

+ Comment chiffres tu les données ? 
+ Quelle techno utilises tu ? 
> JWT, OAuth, XOR, Bearer, Clé publique/privé....

**Les données**
+ Quelle base de données ? Mongo, postgre,... Pourquoi ? 
+ Que vas tu stocker ? Pourquoi ? 
+ Comment peux tu faire pour suivre en temps réel les sous-marins ?
+ Quel serait ton schéma de données ? 
> Faites un peu d'UML et de schéma de données

**Le président**

+ Quelles sont les fonctionnalités nécessaires ? 
> carte, mode hors ligne, notification...

+ Quel techno ? (cordova, app desktop, pwa,....) Pourquoi ?

> Ici vous pouvez faire un bout de code si vous le souhaitez, Mettre des POI sur une carte par exemple. (tri, sort, merge...)

**Le test**

+ Comment testes tu l'ensemble ?
+ Quel(le) framework/techno utilises tu ?
+ Comment vas tu faire une CI du projet ?
+ Comment affiches tu les résultats ?
> test coverage, allure, gitlab ....

+ Coverage ?

**L'équipe**

+ De combien de personnes as tu besoin pour faire tout le système ? 
+ Comment répartis tu l'équipe ? 
+ Où te places tu ? 
> la question sur sa place vous en dira beaucoup sur son esprit d'équipe

> pense-t-il le projet comme une startup ou comme un projet d'Etat industriel ?

## Question annexes 

+ le système est sexy ! les pays de l'UE veuillent se greffer au système comment fait-on ? 
+ attaque de zombie : comment gérer les points d'attaque et la remonté d'infos 
