FROM node:12.2.0
# Create app directory
WORKDIR /usr/src/server
COPY package*.json /usr/src/server
RUN npm install
COPY . /usr/src/server
EXPOSE 9090
CMD [ "node", "server.js" ]