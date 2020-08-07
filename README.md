#Code-source-projet-xml-entrevoisins
#Pour démarrer notre API il vous faut : 
-Un serveur XAMPP ou WAMPP ; 
-démarrer Apache et MySQL ;
-Créer une base de données DBVOISINS avec une table T_VOISINS avec les champs suivants :
	nom varchar;
	adresse varchar;
	numero varchar;
	compte varchar;
	apropos varchar;
	estFavoris boolean; : pour faire d’un voisin un favoris.
	photo varchar; : pour url de la photo d’un voisin.
.
#Les outils pour tester les APIs : POSTMAN ou SOAPUI :
NB : le projet a été réaliser et tester avec serveur XAMPP, nous recommandons XAMPP pour le test.
Il suffit juste de télécharger le dossier «projet-xml-entrevoisins.rar" que nous avons déposé   dans htdocs du serveur XAMPP  et ensuite lancer  POSTMAN ou SOAPUI  utiliser les URL donner dans le document expliquant les APIs  pour lancer les requêtes.
EXEMPLE : GET http://localhost/projet-xml-entrevoisins/public/api/voisins pour lister tous les voisins.

#Les dossiers du projet :
A part les dossiers "public" et "src» qui contiennent les codes sources  de nos APIs et tout ce qui est rapport avec, les autres sont générés lors de l'installation du Framework.
"public" contient :
	htacces.php pour les redirections
	index.php  qui permet de définir les imports de nos differents fichiers.
"src" contient les dossiers «configs" et "routes" dont:
	configs contient DBAcces.php  pour configurer les informations de connexion à la base de données (ip serveur, username, password, dbname ...etc).
	routes qui contient les differentes APIs.

#En cas de problème avec lors du test cela peut être due au framework slim 
il faut installer framework et les dependences vous-même
Commencer par installer composer pour l’installation du FRAMEWORK SLIM et dépendances de PHP.
Aller dans le dossier htdocs de XAMPP ou www de WAMPP créer un dossier par exemple monAppEntreVoisin ouvrez le dossier dans cmd et exécuter la commande suivante :
composer require slim/slim  "^3.12" et en fin copier les dossier public et src du fichier .rar dans monAppEntreVoisin puis lancer POSTMAN ou SOAPUI procéder au test.

