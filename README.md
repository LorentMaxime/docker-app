# docker-app

Pour demarrer l'application en mode developpement :

    docker compose -f docker-compose.dev.yml up --build

le front est disponible à l'adresse http://localhost:3000 (pour regler un soucis d'hot reloading, il ne l'est pas sur le port 8080)

le back (API) est disponible à l'adresse http://localhost:5050

<h2>les différentes commandes Docker</h2>

<h3>docker compose -f docker-compose.dev.yml up --build</h3>

Grâce au fichier docker-compose.yml on peut déclarer les conteneurs comme des services. On peut préciser les options nécessaires au fonctionnement, comme par exemple déclarer les ports et les volumes. On peut créer plusieurs fichiers pour les différents environnements comme la production ou le développement.

<h3>docker compose up</h3>

Docker Compose démarre un conteneur Docker à partir du nom d'une image. L'image est d'abord cherchée en local puis sur DockerHub si elle n'est pas présente.

Docker Compose permet d'automatiser et aussi de versionner les commandes docker run comportant de nombreux arguments. Le conteneur server est capable de résoudre l'url mongodb://mongodb:27017 car le service est nommé mongodb.

<h3>docker image rm</h3>
permet de lister les images Docker en activitées

<h3>docker compose -f docker-compose.dev.yml up</h3>
    
<h3>docker compose -f docker-compose.dev.yml up --build</h3>
chaque modif il faut re builder

<h3>docker compose down</h3>
clos tous les conteneurs actifs
