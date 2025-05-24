# Compte Rendu du Projet – Intercom Bluetooth

## 1. Présentation du projet

Ce projet a consisté à concevoir un **système d’intercom Bluetooth** intégrable dans un casque de moto, utilisant le module **BM83** de Microchip. L’objectif était de permettre une communication audio sans fil avec une interface simple et une bonne qualité audio.

---

## 2. Équipe projet

- **Nom 1** – Rôle (ex. conception PCB, gestion logistique)
- **Nom 2** – Rôle (ex. intégration hardware, tests)
- **Nom 3** – Rôle (ex. documentation, suivi projet)

---

## 3. Matériel utilisé

| Composant                               | Fonction                                 |
|-----------------------------------------|------------------------------------------|
| BM83SM1-00TA                            | Module Bluetooth audio                   |
| Haut-parleurs 40 mm                     | Sortie audio dans le casque              |
| USB-C breakout                          | Chargement et alimentation               |
| Batterie Li-ion 3,7 V                   | Alimentation portable                    |
| Carte PCB custom (sous KiCad)           | Intégration du système                   |

---

## 4. Organisation du projet

Voir le fichier `diagramme_gantt.pdf` dans ce dossier pour la planification complète.

| Étape                    | Dates                | Responsable(s)         |
|--------------------------|----------------------|-------------------------|
| Définition des besoins   | Semaine 1            | Toute l'équipe          |
| Recherche technique      | Semaine 2            | [Nom]                   |
| Conception PCB           | Semaine 3 à 4        | [Nom]                   |
| Commande composants      | Semaine 4            | [Nom]                   |
| Assemblage & tests       | Semaine 5 à 6        | [Nom]                   |
| Finalisation & rendu     | Semaine 7            | Toute l'équipe          |

---

## 5. Choix techniques

- Utilisation du module **BM83** pour éviter le développement d’une stack Bluetooth.
- PCB réalisé avec **KiCad**, à simple couche pour faciliter la fabrication.
- Haut-parleurs en sortie directe avec amplification intégrée.
- Choix de connecteurs USB-C pour la recharge, car standardisé et robuste.

---

## 6. Problèmes rencontrés

- Difficulté à comprendre la documentation de la BM83.
- Délais de livraison sur certains composants.
- Contrainte de place sur le PCB à cause de la forme du casque.
- Nécessité d’outils spécifiques pour le flashage (non utilisé au final grâce au firmware préchargé).

---

## 7. Résultat

Le prototype final fonctionne conformément au cahier des charges minimal :
- Connexion Bluetooth fiable.
- Audio mono clair.
- Recharge par USB-C.
- Intégration possible dans un casque de moto.

---

## 8. Améliorations futures

- Passage à une **sortie stéréo**.
- **Réduction active du bruit** par traitement numérique.
- Ajout d’un **afficheur OLED** pour le retour utilisateur.
- Communication entre casques (intercom multi-utilisateur).

---

## 9. Annexes

- [cahier_des_charges.md](./cahier_des_charges.md)
- [composants_commandés.md](./composants_commandés.md)
- [diagramme_gantt.pdf](./diagramme_gantt.pdf)
