# Usa una imagen base de Node.js
FROM node:22-alpine

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el package.json y package-lock.json (si existe) para instalar las dependencias
COPY package*.json ./

# Instala las dependencias
RUN npm install

# Copia el resto de los archivos de la aplicación
COPY . .

# Compila la aplicación React para producción
RUN npm run build

# Comando para iniciar la aplicación (esto depende de cómo configures tu aplicación)
CMD ["npm", "start"]
