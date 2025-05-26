1. Introduction

Ce projet a consisté à concevoir un système d’intercommunication Bluetooth embarqué dans un casque de moto, reposant sur le module BM83 de Microchip. L’objectif principal était de permettre une communication audio sans fil entre motards, avec une interface simple, une bonne qualité audio, et une intégration physique adaptée aux contraintes d’un casque.

2. Équipe Projet

Nom	                                    Rôle
Julien Burger , Nuvaragan Kulasingam	- Conception du circuit imprimé (PCB), gestion logistique

Julien Burger , Bilal yousfi -	Intégration hardware, tests fonctionnels

Ryad Kacha , Cyrille Velanganni , Yacoub Abdoulkader -	Rédaction de la documentation, suivi de l’avancement projet, rédaction du GitHub

3. Organisation et Planification

La planification du projet a été organisée selon un diagramme de Gantt détaillé, incluant toutes les phases : étude, conception, prototypage, tests.
![Diagramme de Gantt](./Weekly%20Gantt%20Chart%20Intercom%20Bluetooth.png)

  
4. Choix Techniques

Les choix techniques ont été faits dans une optique d'efficacité, de simplicité d'intégration, et de compatibilité :
Module Bluetooth : utilisation du BM83 pour bénéficier d’une stack Bluetooth préintégrée, évitant le développement logiciel complexe.
Circuit imprimé (PCB) : conçu avec KiCad, en 4 couches pour la première version et en 2 couches pour la seconde version, afin de simplifier la fabrication manuelle.
Connectique : utilisation d’un connecteur USB-C pour la recharge 
Sortie audio : amplification intégrée et haut-parleurs connectés directement.
Alimentation : batterie lithium-polymère rechargeable via USB-C.
  
5. Difficultés Rencontrées

Le projet a fait face à plusieurs obstacles techniques et logistiques :
Documentation technique complexe du module BM83, nécessitant un temps d’apprentissage important.
Délais de livraison de certains composants critiques.
Contrainte spatiale sur le PCB due à l’espace limité dans un casque de moto.
Flashage initial non réalisé en raison de l’existence d’un firmware préchargé fonctionnel.
  
6. Résultats Obtenus

Le prototype final est pleinement fonctionnel et respecte le cahier des charges minimal :
Connexion Bluetooth stable et fiable.
Recharge via USB-C opérationnelle.
Intégration physique réussie dans un casque moto standard.
  
7. Pistes d’Amélioration

Des évolutions futures ont été identifiées pour améliorer les performances et les fonctionnalités :
Passage à une sortie audio stéréo.
Intégration d’un système de réduction active de bruit (filtrage DSP).
Ajout d’un afficheur OLED pour afficher l’état de connexion ou le niveau de batterie.
Développement d’un mode intercom multi-utilisateur, permettant la communication entre plusieurs casques.

8. Annexes

[Cahier des charges](./Gestion%20de%20projet/cahier_des_charges.md)

[Liste des composants commandés](./Gestion%20de%20projet/composants.md)

[Diagramme de Gantt](./Gestion%20de%20projet/Weekly%20Gantt%20Chart%20Intercom%20Bluetooth.png)


