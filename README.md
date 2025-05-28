# Intercom Bluetooth pour Moto

Bienvenue ! Ce dépôt contient **tout le nécessaire pour reproduire notre projet** d'intercom Bluetooth pour moto.
Voici la présentation du projet : ""
---

## Description du Projet

Ce projet est un système de communication audio sans fil entre deux casques de moto. Il permet :
- La lecture de musique stéréo en Bluetooth
- La communication vocale entre deux usagers via microphones numériques
- Le contrôle du module via des LEDS et interrupteurs
- Une alimentation USB-C standardisée
- Une consommation optimisée et un encombrement réduit

---

## Démarche de Conception

### Étape 1 – Analyse des besoins

Nous avons commencé par rédiger un cahier des charges (voir Gestion de projet/cahier_des_charges.md) définissant :
- La nécessité d’une communication bidirectionnelle claire
- L’autonomie et la simplicité d’utilisation
- Une interface Bluetooth stable et performante
- Un design compact pour intégration dans un casque

### Étape 2 – Recherche de solutions Bluetooth

Nous avons comparé plusieurs options :
- ESP32 avec gestion audio
- Solutions séparées Bluetooth + CODEC I2S

Pourquoi le *BM83* a été retenu

Le *BM83* s’est imposé pour plusieurs raisons :
- Solution tout-en-un : gestion Bluetooth, audio, micro, DSP intégré
- Support complet de l’I2S numérique : idéal pour les microphones ICS-43434
- Pas de microcontrôleur externe nécessaire pour l’audio
- Configuration simple via UART
- Le BM83 embarque une stack Bluetooth 5.0, un contrôleur audio, un DSP intégré, et la gestion micro/haut-parleur

Après avoir choisi le BM83, nous avons conceptionné via KiCad une première version de la carte, voici un aperçu du PCB : [o](./Hardware/pcb v1.pdf)
Si vous désirez reproduire ce projet, vous devriez télécharger en amont les libraires d'empreintes sur le schéma KiCad.
Après celà nous avons essayé de flasher la carte pour pouvoir établir une connexion Bluetooth entre un appareil téléphonique et la carte Intercom , cependant rien ne fonctionnait , ce fût un échec dû au mauvais choix des composants .
Nous avons analysé d'où provenaient les failles en relisant les datasheets  en portant une attention particulière sur les étapes qu'il faut réaliser et les différents composants nécessaires à la conception du PCB.
Par la suite nous avons conçu une seconde carte, et avec ça nous avons flashé cette dernière grâce à un software fourni par le constructeur du BM83 "[
BM83 Firmware Update via USB](https://www.youtube.com/watch?v=SPlbVVXS5hs)" et "[
BM83 Stereo Embedded Demo](https://www.youtube.com/watch?v=FLCs_W62KlI)" , nous avons suivi les étapes de cette vidéo.


**Par comparaison** :
- L’ESP32 Audio aurait nécessité beaucoup plus de code, d’énergie et de composants externes.
- Les solutions à base de CODEC analogique/I2S séparés complexifient le PCB.

En résumé : le **BM83 est fiable, documenté, compact, et parfaitement adapté à un intercom Bluetooth embarqué**.


### Annexes et liens utiles :

Pour consulter l’organisation du projet et le suivi des séances, voir le dossier [Gestion de projet](./Gestion%20de%20projet/)

Pour consulter le dossier contenant les deux versions de pcb en .zip, voir le dossier [Hardware](./Hardware/)

Pour consulter le dossier contenant les datasheets et la partie Software (firmaware), voir le dossier [Datasheets](./Datasheets/) et [Software](./Software).


---
