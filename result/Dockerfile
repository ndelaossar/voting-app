FROM node:18-alpine

USER node

WORKDIR /app

COPY ["package.json", "package-lock.json*", "./"]

RUN npm ci

COPY --chown=node:node . .

EXPOSE 3000
CMD [ "node", "server.js" ]