# CritiPixel

## Installation
Dans un premier temps, installer les dépendances :
```bash
composer install
```

Pensez à créer un fichier `.env.local` si nécessaire pour configurer l'accès à la base de données. 

Vous pouvez aussi utiliser **Docker compose** si vous le souhaitez, une base de données y est configuré.

Il ne vous reste plus qu'à créer la base de données :
```bash
symfony console doctrine:database:create
symfony console doctrine:migrations:migrate
symfony console doctrine:fixtures:load
```