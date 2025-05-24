# 🏍️ Intercom Bluetooth pour Moto

Bienvenue ! Ce dépôt contient **tout le nécessaire pour reproduire notre projet** d'intercom Bluetooth pour moto.
---

## 🧩 Description du Projet

Ce projet est un **système de communication audio sans fil** entre deux casques de moto. Il permet :
- La **lecture de musique stéréo** en Bluetooth
- La **communication vocale** entre deux usagers via microphones numériques
- Le **contrôle du module** via des LEDS et interrupteurs
- Une **alimentation USB-C standardisée**
- Une consommation optimisée et un encombrement réduit

---

## 💡 Démarche de Conception

### Étape 1 – Analyse des besoins
Nous avons commencé par rédiger un **cahier des charges** (voir `Gestion_de_projet/cahier_des_charges.md`) définissant :
- La nécessité d’une communication bidirectionnelle claire
- L’autonomie et la simplicité d’utilisation
- Une interface Bluetooth stable et performante
- Un design compact pour intégration dans un casque

### Étape 2 – Recherche de solutions Bluetooth
Nous avons comparé plusieurs options :
- ESP32 avec gestion audio
- Solutions séparées Bluetooth + CODEC I2S

### Étape 3 – Pourquoi le **BM83** a été retenu

Le **BM83** s’est imposé pour plusieurs raisons :
- **Solution tout-en-un** : gestion Bluetooth, audio, micro, DSP intégré
- **Support complet de l’I2S numérique** : idéal pour les microphones ICS-43434
- **Pas de microcontrôleur externe nécessaire** pour l’audio
- **Configuration simple via UART**


**Par comparaison** :
- L’ESP32 Audio aurait nécessité beaucoup plus de code, d’énergie et de composants externes.
- Les solutions à base de CODEC analogique/I2S séparés complexifient le PCB.

👉 En résumé : le **BM83 est fiable, documenté, compact, et parfaitement adapté à un intercom Bluetooth embarqué**.

---
