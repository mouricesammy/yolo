FROM node:19-alpine
WORKDIR /app
COPY package*.json .
RUN npm install
COPY . .
RUN npm run
EXPOSE 5050
CMD [ "node", "server.js"]