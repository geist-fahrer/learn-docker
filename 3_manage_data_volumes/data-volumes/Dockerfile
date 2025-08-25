FROM node:lts-alpine3.22

WORKDIR /app

COPY package.json .

RUN npm install

ENV PORT=80

COPY . .

EXPOSE $PORT

CMD ["npm", "start"]