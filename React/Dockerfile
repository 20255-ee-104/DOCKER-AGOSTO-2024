# Usa una imagen base de Node.js específica, por ejemplo, Node.js 18 con Alpine para una imagen ligera
FROM node:18-alpine

# Establece el directorio de trabajo dentro del contenedor
WORKDIR /app

# Copia el archivo package.json y package-lock.json (si existe)
COPY package.json package-lock.json ./

# Instala las dependencias del proyecto
RUN npm install

# Copia el resto de la aplicación al directorio de trabajo en el contenedor
COPY . .

# Expones el puerto en el que la aplicación se ejecutará (opcional, dependiendo de la aplicación)
EXPOSE 3000

# Comando para ejecutar la aplicación
CMD ["npm", "start"]
