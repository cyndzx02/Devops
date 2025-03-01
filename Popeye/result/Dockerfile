FROM node:20-alpine

COPY package.json .

COPY . .

RUN npm install

EXPOSE 80

CMD ["node", "server.js"]