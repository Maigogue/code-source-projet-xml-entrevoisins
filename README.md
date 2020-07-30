# code-source-projet-xml-entrevoisins
Pour démarrer notre API  il vous faut: 
-Un serveur XAMPP ou WAMPP; 
-démarrer Apache ;
-Créer une base de données avec  les champs suivantes:
  -nom varchar
  -adresse varchar
  -numero varchar
  -compte varchar
  -apropos varchar
  -estFavoris boolean
  -photo varchar
NB: Pour faciliter les testes il faut nommé la table  t_voisins  car ce le nom est utiliser dans les rêquetes des APIs.

-Un outil pour tester les APIs POSTMAN ou SOAPUI
NB: le projet  a été réaliser et tester avec serveur XAMPP , nous récommandons XAMPP pour le  test.
il suffit juste de copier le  dossier  "projet-xml-entrevoisins"  dans htdocs du serveur XAMPP  et ensuite lancer  POSTMAN ou SOAPUI  utiliser les URL donner dans le document expliquant les APIs  pour lancer les requêtes.
EXEMPLE : GET http://localhost/projet-xml-entrevoisins/public/api/voisins pour  lister tous les voisins.

Les dossiers du projet:
A part  les dossiers "public" et "src"  qui contienent les codes sources  de nos APIs et tout ce qui est rapport avec, les autres sont générés lors de l'installation du Framework.
"public" contient:
-htacces.php pour les redirections
-index.php  qui permet de définir les imports de nos differents fichiers.
"src" contient  les dossiers  "configs" et "routes" dont:
-configs contient DBAcces.php  pour configurer les informations de la base de données (ip serveur, username, password, dbname ...etc).
-routes qui contient les differentes APIs.
