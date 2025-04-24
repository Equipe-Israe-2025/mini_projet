FROM node:latest

WORKDIR /app

COPY package*.json ./
RUN npm ci --quiet 
#npm clean install avec --quiet qui réduit les messages logs 


COPY . .

EXPOSE 3000

USER node

CMD ["node", "app.js"]
