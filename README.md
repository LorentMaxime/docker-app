# docker-app

Pour demarrer l'application en mode developpement :

    docker compose -f docker-compose.dev.yml up --build

le front est disponible à l'adresse http://localhost:3000 (pour regler un soucis d'hot reloading, il ne l'est pas sur le port 8080)

le back (API) est disponible à l'adresse http://localhost:5050
