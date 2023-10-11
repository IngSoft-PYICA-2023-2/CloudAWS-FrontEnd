# Utilizamos una imagen de Node.js
FROM node:16

# Establecemos el directorio de trabajo
WORKDIR /app

# Copiamos los archivos necesarios al directorio de trabajo
COPY package.json package-lock.json /app/
RUN npm install

COPY . /app/

# Puerto en el que correrá la aplicación
EXPOSE 3000

# Comando para iniciar la aplicación
CMD ["node", "src/server.js"]
