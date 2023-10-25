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



• Travail de l'après-midi : établir une liste de classe et sous classe qui permettront à notre DM de fonctionner et de passer les différents Units Tests

**1) Classe MachineMaintienDuCoeur**
C'est la classe principale, elle représente la machine dans son ensemble et contrôle les liens entre les différents composants.

**2) CLasse Capteurs**
Cette classe permettra de vérifier les paramètres de tous nos différents capteurs
On va donc créer une sous-classe par capteurs nécessaires au bon fonctionnement de notre DM

   **Sous-classe DétecteurTempérature**
   Cette sous-classe permet de gérer le contrôle de la température du coeur.

   **Sous-classe DétecteurHumidité**
   Cette sous-classe permet de gérer le taux d'humidité au sein de la machine.
   Taux entre 30 et 60%.

   **Sous-classe DétecteurPression**
   Cette sous-classe permet de gérer le contrôle de la pression au sein de la machine et vérifier qu'on ne dépasse jamais les seuils préconisés.


**3) Classe Sécurité**
Cette classe va permettre de gérer tous les systèmes de sécurité du dispositif
Elle est reliée à la classe Capteurs.

   **Sous-classe Alarme**
   Cette classe gèrera les différentes alarmes nécessaires en cas de variations de température, pression, humidité... Dès que nos capteurs détecteront des seuils hors des plages acceptables, elle permettra de déclencher une alarme et donc informer le personnel médical.

   **Sous-classe ArretUrgence** 
   Cette classe s'occupera des protocoles d'arrêt d'urgence. Elle sera capable de mettre la machine hors tension en cas d'urgence.


**4) Classe Prévention**
Cette classe concerne les différents diagnostics et maintenances à réaliser afin de garantir le bon fonctionnement de la machine.

   **Sous-classe Maintenances**
   Elle gère les tâches de maintenances préventive : elle sera capable de planifier et effectuer des opérations de maintenances régulières. Elle sera également capable de prévenir les utilisateurs lorsqu'il est temps de réaliser une maintenance plus profonde.

   **Sous-classe Diagnostics**
   Cette sous-classe gère les fonctions d'auto-diagnostics (réalisation de tests internes, détection des défaillances...)


**5) Classe Communication**
Cette classe s'occupera des protocoles de communication avec d'autres systèmes médicaux : elle sera capable d'envoyer et recevoir des données de l'extérieur.
