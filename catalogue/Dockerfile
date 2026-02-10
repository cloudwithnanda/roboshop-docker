FROM node:20-alpine

WORKDIR /app

# Needed only if native modules exist
RUN apk add --no-cache python3 make g++

COPY package.json ./
RUN npm install

COPY *.js ./

CMD ["node", "server.js"]
