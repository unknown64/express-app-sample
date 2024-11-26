# Express App Cluster

## Configuration des services
1. Cloner le dépôt :  

git clone <URL_DU_DEPOT>


2. Créer les secrets pour la base de données :  

echo "your_db_password" | docker secret create db_password - echo "your_db_user" | docker secret create db_user -


3. Déployer la stack avec Docker Compose :  

docker stack deploy -c docker-compose.yml express-app-stack


4. Vérifier l’état des services :  

docker service ls
