DOCKER START --------------------------

docker compose down --remove-orphans | Retire tous les conteneurs même ceux qui ne sont pas dans le docker compose
docker compose up --build | Resoudre les problatiques liées au démarrage des images

HOT RELOAD ----------------------------

Ajouter "WATCHPACK_POLLING=true" dans la mention start du package.json
Ajouter dans le docker-compose.yml "environment: - CHOKIDAR_USEPOLLING=true"
