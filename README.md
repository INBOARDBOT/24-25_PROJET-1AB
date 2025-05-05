# 🏍️ Intercom Bluetooth pour Moto

Ce dépôt contient **tout le nécessaire pour reproduire notre projet** d'intercom Bluetooth pour moto. 

## Description du Projet

Ce projet est un **système de communication Bluetooth pour moto**, permettant entre autres :
- Une communication audio entre deux casques
- La lecture de musique en stéréo
- L’utilisation d’un microphone numérique
- Des LED d'indication et interrupteurs pour le contrôle
- Une compatibilité avec l’alimentation USB-C

Afin de réaliser ce projet, nous avons utilisé le BM83, un module Bluetooth qui offre une solution intégrée, fiable, documentée et optimisée pour l’audio Bluetooth, parfaite pour un projet comme un intercom moto où la compacité, l’autonomie, et la qualité audio sont prioritaires. Il gère des microphones numériques I²S, ce qui simplifie l'intégration des micros ICS-43434 sans passer par des convertisseurs analogiques ou des CODECs externes complexes. Le BM83 intègre également son propre DSP audio, donc on n'a pas besoin de gérer des flux audio lourds avec un MCU externe.
Tout compte fait, l'utilisation de la BM833 permet de réduire la consommation, par rapport à d'autres alternatives (comme l'ESP32 Audio), de ne pas avoir de créer de code pour notre solution et également pour avoir un schéma PCB moins chargé.


## 🗂️ Organisation du Dépôt

Voici comment le dépôt est structuré :
 - Hardware : contient le pcb
 - Software : contient le firmware du BM83 (n'ayant pas écrit de nouveau code pour notre projet)
 - Datasheets : contient toute la documentation des composants utilisés
 - Gestion de projet : contient "suivi.md", qui contient toutes les étapes du projet, séance par séance afin de réaliser le cahier des charges


 



