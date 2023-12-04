Ce cahier des charges, par rapport à l'état de l'art réalisé et aux contraintes définies (Cf documentation), doit décrire le matériel et spécifier les critères choisis par rapport à nos besoins.  

### 1. **Introduction**

#### 1.1 **Objectif du Projet**
Le but de ce projet est de concevoir, développer et tester un système de transport innovant et fiable pour les cœurs implantables, assurant leur préservation optimale pendant le transit pour les transplantations cardiaques.

#### 1.2 **Contexte**
Le transport sécurisé des cœurs implantables est d'une importance vitale pour le succès des transplantations cardiaques. Cette machine de transport vise à réduire le temps de transfert, à maintenir une température et une humidité constantes, et à garantir la viabilité de l'organe.

### 2. **Spécifications Techniques**

   **Cf document "Constantes et Contraintes".** et **"Units tests.md"** Ces document reprennent toutes les contraintes techniques avec les seuils de validation des capteurs de température, le taux d'humidité, la fréquence cardiaque...

  Maintenir le cœur en état de battement pendant tout le transport. Cela permet de maintenir un flux sanguin et une oxygénation adéquats, minimisant ainsi l'ischémie froide et préservant la fonction cardiaque.
  
  Evaluation en temps réél --> surveillance de la fonction cardiaque, du débit sanguin, de l'oxygénation et d'autres paramètres permettant à l'équipe médical de réagir rapidement. 
  
Permettre une durée de transport prolongée --> essentiel lorsque les donneurs et les receveurs se trouvent à une distance considérable les uns des autres = cela augmente les possibilités de transplantation en élargissant la portée géographique.
  
  Fournir un environnement de transport optimal pour chaque cœur --> réduire la variabilité entre les donneurs + améliorer la qualité de l'organe transplanté.

### **Valeurs pour les capteurs :**

#### **Plage de Température Acceptable :**
- **Plage de Température Cible :** 4°C à 8°C (pour le transport du cœur dans un état de préservation pour la greffe).
- **Précision des Capteurs :** ±0.1°C.

#### **Plage de Pression Acceptable :**
- **Plage de Pression Cible :** 70 mmHg à 110 mmHg (pour maintenir une pression artérielle physiologique).
- **Précision des Capteurs :** ±2 mmHg.

#### **Temps d'Arrêt d'Urgence :**
- **Temps Maximal Avant Arrêt d'Urgence :** 2 secondes (pour une réponse rapide aux situations critiques).

#### **Fréquence de Maintenance Préventive :**
- **Fréquence de Maintenance :** Tous les 6 mois (pour des performances constantes et sûres).

#### **Sécurité de la Communication :**
- **Cryptage des Données :** Protocole AES-256 (pour assurer une communication sécurisée).

#### **Durée Maximale de Transport :**
- **Durée Maximale de Transport Autorisée :** 6 heures (pour maintenir la viabilité de l'organe).

#### **Seuils d'Alarme :**
- **Seuils de Température Alarmante :** Inférieure à 2°C ou supérieure à 10°C (pour signaler des variations extrêmes).
- **Seuils de Pression Alarmante :** Inférieure à 60 mmHg ou supérieure à 120 mmHg.

Il y a aussi la contrainte des solutions dans lesquelles on plonge le coeur pour préserver l'organe : 

#### **Solutions de Préservation d'Organe Améliorées :**

1. **Solutions d'Hypothermie et de Conservation à Base de Custodiol :** Ces solutions contiennent des composants spécifiques qui aident à préserver la viabilité des organes pendant le transport en réduisant leur température et en fournissant des nutriments et des agents anti-coagulants.

#### **Recherche sur les Organes Cultivés :**

La recherche sur les organes cultivés en laboratoire, souvent appelée ingénierie tissulaire ou bioprinting, vise à créer des organes artificiels en utilisant des cellules humaines et des biomatériaux. Bien que cette technologie soit encore en développement, elle offre un immense potentiel pour remédier aux problèmes de pénurie d'organes et de compatibilité.

#### **Optimisation des Procédures de Greffe :**

L'expérience des équipes médicales, les protocoles chirurgicaux améliorés et l'optimisation des soins post-opératoires jouent également un rôle crucial dans le succès des transplantations d'organes.


#### 2.1 Conditions de Stockage
Le système doit maintenir une température entre 36 et 38 °C et une humidité optimale pour garantir la préservation du cœur implantable pendant le transport.

#### 2.2 Alimentation
La machine doit être alimentée par une source d'énergie interchangeable et fiable, capable de fonctionner en continu pendant au moins 24h sans interruption.

#### 2.3 Technologie de Refroidissement
La machine doit être équipée d'un système de refroidissement avancé, basé sur [indiquez la technologie utilisée], pour maintenir une température stable à l'intérieur de la boîte de transport.

#### 2.4 Système de Surveillance
La machine doit être équipée de capteurs de haute précision pour surveiller en temps réel la température, l'humidité et d'autres paramètres critiques. Ces données doivent être accessibles aux professionnels de la santé via une interface conviviale.

Chaque capteurs doit être définies. 

### 3. **Fonctionnalités**
   
#### 3.1 Sécurité
- La machine doit comporter un système de verrouillage biométrique ou électronique pour empêcher tout accès non autorisé.
- Un système d'alerte automatique doit être intégré pour signaler toute anomalie ou variation soudaine des conditions internes.

#### 3.2 Facilité de Maintenance
- La machine doit être conçue de manière modulaire pour permettre un démontage facile aux fins d'entretien ou de réparation.
- Un système d'autodiagnostic avancé doit être intégré pour détecter les problèmes potentiels et générer des rapports d'état.

### 4. **Conformité Réglementaire et Sécurité**

#### 4.1 Conformité aux Normes

La machine doit être conforme aux normes et réglementations médicales internationales, y compris celles définies par l'OMS et la FDA, garantissant ainsi son utilisation sûre et légale.


### 5. **Échéancier**

**Cf diagramme de Gantt**
