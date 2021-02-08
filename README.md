## 25/05/2020 initialisation du projet du Deckbuilder Yu-Gi-Oh

# Présentation du projet : 
Le projet a pour but d'être un créateur de deck de carte Yu-Gi-Oh avec un bibliothèque évolutive . C'est a dire que si vous recherchez une carte qui n'est pas existante dans notre BDD (si la carte est nouvelle ou inexistante dans la BDD).La carte et toutes ses données y sont enregistré via une API.

# Liste des étapes pour créer le symfony : 

- squelette de symfony :
```
composer create-project symfony/website-skeleton deckbuilder_yugioh ^4.4.*
```
- appache-pack : 
``` 
composer require symfony/apache-pack
```
- extension de doctrine : 
```
composer require beberlei/doctrineextensions
```
- orm-fixtures
```
composer require --dev orm-fixtures
```

# Initialiser le projet chez sois :
- 1 
````
composer install
````
- 2 
```` 
php bin/console doctrine:database:create
````
- 3
````
php bin/console doctrine:migrations:migrate
````
