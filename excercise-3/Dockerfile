FROM node:9.11.2-alpine

COPY package.json package.json

RUN npm install

COPY . .

EXPOSE 3000

CMD npm start

