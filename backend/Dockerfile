FROM node:18-alpine

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install

COPY . .

RUN npm run build

EXPOSE 3000

# Roda o NestJS em modo de observação (hot reload)
CMD ["npm", "run", "start:dev"]