
# Projet DEVOPS IPSSI

Vous allez faire un projet DevOps.

# I- Sujet

## Applications 

L'objectif est l'intégration des applications Car.API (dot net core) et Auto (Angular) dans un CI/CD Azure DevOps.

## Ce qui est fournis

Pour ce projet, je vous fournis le code source de 2 applications. Les applications sont disponibles sur le [git](https://github.com/bart120/projetipssi).
Description des apps:
- Auto => application Angular
- Car.API => service API REST fournissant des données d'une base de données.

## Repository

Vous devez créer 2 projets Azure DevOps puis récupérer les sources de chaque application afin de les mettre dans un repository Azure DevOps.

## Auto

Application Angular.
Le pipeline de cette application devra contenir les éléments suivants:
- Build
- Tests unitaires
- Qualité de code et publication du rapport de qualité dans Sonar Cloud
- Publier l'artefact au format NPM
- Création d'une image Docker de l'application
- Publication de l'image Docker dans le Docker hub

## Car.API

Service API REST fournissant des données d'une base de données.
Le pipeline de cette application devra contenir les éléments suivants:
- Build
- Tests unitaires
- Déploiement de la base de données
- Qualité de code et publication du rapport de qualité dans Sonar Cloud
- Publier l'artefact au format Nuget
- Création d'une image Docker de l'application
- Publication de l'image Docker dans le Docker hub

## Base de données

L'API Car.API utilise en base de données MS Sql Serveur via Entity Framework.
Il y a déjà une migration prête dans l'application. Vous devrez donc éxécuter les migrations afin de mettre à jour la structure de la base de données.
La chaine de connection se trouve dans le fichier appsettings.json
Vous devrez avoir créer au préalable une base de données SqlServer dans Azure. (Si votre compte Azure est épuisé, je vous fournirai une base de données Azure).

## Services connectés

Pour les artefacts, vous pouvez les déployer sur Azure DevOps, soit sur [npmjs.org](https://www.npmjs.com/) et [nuget.org](https://www.nuget.org/)
Pour la qualité de code, publier les résltats sur [Sonar Cloud](https://sonarcloud.io/).
Pour les images Docker, elles seront publiées sur le [docker hub](https://hub.docker.com/).

## Publication

Chaque artefact et image Docker devra être taguer avec la version de Build.

# Groupes et fonctionnement

Le projet est a faire en groupe de 2 personnes (ou seul).
Tous les groupes seront définis en cours, sous la supervision de l'enseignant. Les groupes s'enregistrent avec un nom de groupe ainsi que les noms de leurs membres.

Toute inscription est définitive.  Les étudiants ne sont pas autorisés, par la suite, à changer de groupe.

Au sein d'un groupe, les étudiants se répartiront les tâches pour le projet, de façon équitable.

# Rendu

Le rendu se fera le vendredi 18 juin 2021.

Les rendus doivent figurer sur un seul compte par groupe.
Le mail de rendu est vincent.leclerc@ecole-ipssi.net
Les fichiers rendus doivent contenir
  - Les fichiers (yaml) et documents techniques du projet.
  - Un AUTHORS.TXT listant les membres du groupe (prénom, nom), à raison d'un par ligne.  Il liste ensuite les responsabilités effectives de chacun dans le groupe.
Le sujet du mail doit contenir votre section ainsi que le nom du projet.
Les fichiers rendus peuvent aussi comprendre: 
  - Des documents de recherche créés pour le projet et fournissant plus de détails pour l'enseignant.
Pour tout autre type de fichier, veuillez demander à l'enseignant si son inclusion est appropriée.