FROM nginx:alpine

# Supprime la page d'accueil par défaut
RUN rm -rf /usr/share/nginx/html/*

COPY index.html /usr/share/nginx/html/

# le port 80 d'écoute nginx
EXPOSE 80
