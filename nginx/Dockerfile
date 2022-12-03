# Je part d'une image de base : node:16 
FROM node:16 as builder
# Je définie un répertoire 
WORKDIR /app
# Je copie mon code dans mon container
COPY ./code .
# Installation / build
RUN yarn install
RUN yarn build

# Configuration nginx
FROM nginx:1.21.0-alpine as production
COPY --from=builder /app/build /usr/share/nginx/html
COPY nginx.conf /etc/nginx/conf.d/default.conf

# Démarrage
EXPOSE 80
CMD ["nginx", "-g", "daemon off;"]