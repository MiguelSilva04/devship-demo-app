# usar uma imagem oficial do node mais enxuta para reduzir vulnerabilidades
FROM node:22-alpine

# escolher a working directory
# WORKDIR /app

# copiar o package.json e instalar as dependencias
COPY package*.json ./
RUN npm ci

# copiar o resto da app
COPY . .

# expor a porta 3000
EXPOSE 3000

# startar a app
CMD ["npm","start"]
