# Utiliser une image de base pour Node.js
FROM node:14-alpine

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package*.json ./

# Installer les dépendances
RUN npm install

# Copier le reste des fichiers de l'application
COPY . .

# Exposer le port 4000 (adapter pour chaque service)
EXPOSE 4002

# Démarrer l'application
CMD ["npm", "start"]