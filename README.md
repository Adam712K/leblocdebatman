# Projet Le Blog de Batman

### Cloner le projet

```
git clone https://github.com/Adam712K/leblocdebatman.git
```

### Déplacer le terminal dans le dossier cloné
```
cd leblogdebatman
```

### Installer les vendors (pour recréer le dossier vendor)
```
composer install
```

### Création base de données
Configurer la connexion à la base de données dans le fichier .env (voir cours), puis taper les commandes suivantes :
```
symfony console doctrine:datebase:create
symfony console doctrine:migration:migrate
symfony console doctrine:fixtures:load
```
### Création des fixtures 
```
symfony console doctrine:fixtures:load
```

Cette commande créera : 
* Un compte admin (email: a@a.a , password : 'aaaaaaaaA7/')
* 10 compte utilisateurs (email aléatoire , password : 'aaaaaaaaA7/')
* 200 articles

### Installation fichiers front-end des bundles (CKEditor)
```
symfony console assets:install public
```

### Lancer le serveur
```
symfony serve
```