
Commande de lancement  : docker compose up 
Création d'une image multi stage pour le front end pour lancé uniquement le code compilé et d'avoir une image plus légère.
Le front et d'abord compilé dans une première image puis le build est copié dans une seconde image nginx pour la mettre en exposition.
Création d'une autre image docker basé sur une version Node Alpine pour executé le backend.
Dans le docker compose on déclare les différents chemin de docker file à utilisé et on déclare l'utilisation d'une base de données MongoDB.
Dans la déclaration du back on ajoute un lien vers la base de données Mongo en indiquant le nom du service en tant que lien qui servira comme 
DNS de la base de données.
Ont dis egalement que le conteneur du back end doit attendre l'execution du conteneur de Mongo a l'aide du depends_on puis on déclare les ports des différents services.
