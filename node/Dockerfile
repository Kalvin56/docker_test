# Je part d'une image de base : node:16 
FROM node:16
# Je définie un répertoire 
WORKDIR /app
# Je copie mon code dans mon container
COPY ./code .
# Installation / build
RUN yarn install
RUN yarn build
EXPOSE 3000
# Démarrage
CMD [ "npx", "serve", "build" ]