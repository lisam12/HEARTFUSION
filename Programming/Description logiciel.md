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