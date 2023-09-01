FROM node:16

WORKDIR /usr/src/app

COPY package*.json .

RUN npm install

COPY . .

EXPOSE 3001

# Define the command to start the app
CMD ["node", "server"]