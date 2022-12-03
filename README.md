# Informations

Mise en place d'un serveur web de 3 manières différentes :
  - apache
  - nginx
  - node

# Installation

`cd apache`  
`docker-compose up -d`    
Résultat : http://localhost:8090/

`cd nginx`  
`docker-compose up -d`    
Résultat : http://localhost:3000/

`cd node`  
`docker-compose up -d`  
Résultat : http://localhost:3000/

# Commandes utiles

`docker ps` : voir mes container actifs  
`docker ps --all` : voir tout mes container  
`docker-compose down` : stopper un container  