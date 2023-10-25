Pour le projet on ne code pas, on doit simlpement décrire les classes du code + les tests unitaires. On peut parler de classe sous classe si certaines sont reliées. 
+ il faut penser à détailler comment elles sont reliées si c'est le cas. 

Pour les classes du code par exemple : 
Classe détectuer de Température : Si la température est inférieur à 8 degrès on ne fait rien, si elle dépasse le seuil de 8.6degrès on refroid le coeur. 
Classe détecteur d'humiduté : ....
Par exemple on aura la classe capteurs qui aura comme sous classe : détecteur temp et détecteur humidité

Unit Test : On teste la séquence dans des circonstances variées. Par exemple pour IRM, si on met un FOV à 100%, vérifier si tout s'affiche bien sur tous les IRMS.
Par exemple pour les programmes pythons, quelles librairies utilisées, si on change de version, si on change de librairie. Mouvance de l'intégration continue.
Ce sont des programmes qui testent nos programmes.
Si on veut injecter plus que prévu sur une pompe à injection, il faut qu'elle dise non. 

La conception logicielle d'une machine comme TransMedics implique la création de classes et de sous-classes qui représentent les différents composants et fonctionnalités de la machine. Voici un exemple simplifié de certaines classes et sous-classes que vous pourriez considérer dans la conception logicielle d'une telle machine :

1. **Classe MachineDeMaintienDeCoeur :**
   - Cette classe représente la machine dans son ensemble et peut contenir des méthodes et des propriétés pour contrôler les différents composants.

2. **Sous-classes pour les Composants Principaux :**
   - **Classe SystemeDeControleDeTemperature :**
     - Cette classe gère le contrôle de la température du cœur. Elle pourrait avoir des méthodes pour régler la température et surveiller les capteurs de température.

   - **Classe SystemeDeControleDePression :**
     - Cette classe gère le contrôle de la pression dans la machine. Elle pourrait avoir des méthodes pour régler la pression et surveiller les capteurs de pression.

   - **Classe SystemeDeCommunication :**
     - Cette classe gère les protocoles de communication avec d'autres systèmes médicaux. Elle pourrait avoir des méthodes pour envoyer et recevoir des données.

3. **Sous-classes pour les Fonctionnalités de Sécurité :**
   - **Classe SystemeDAlarme :**
     - Cette classe gère les alarmes en cas de variations de température ou de pression hors des plages acceptables. Elle pourrait avoir des méthodes pour déclencher des alarmes et informer le personnel médical.

   - **Classe SystemeDArretUrgence :**
     - Cette classe gère les protocoles d'arrêt d'urgence. Elle pourrait avoir des méthodes pour mettre la machine hors tension en cas d'urgence.

4. **Sous-classes pour la Maintenance et les Diagnostics :**
   - **Classe SystemeDiagnostics :**
     - Cette classe gère les fonctions d'auto-diagnostic. Elle pourrait avoir des méthodes pour effectuer des tests internes et détecter les défaillances.

   - **Classe SystemeDeMaintenancePreventive :**
     - Cette classe gère les tâches de maintenance préventive. Elle pourrait avoir des méthodes pour planifier et effectuer des opérations de maintenance régulières.
